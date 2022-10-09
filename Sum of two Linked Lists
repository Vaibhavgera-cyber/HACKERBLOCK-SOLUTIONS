#include<iostream>
#include<bits/stdc++.h>
using namespace std;
class Node{
    public:
	int data;
	Node*next;
	Node(int val){
	    data=val;
		next=NULL;
	}
};
void insertAtTail(Node*&head,int data){
	Node*node=new Node(data);
	if(head==NULL){
		head=node;
		head->next==NULL;
	}
	else{
		Node*temp=head;
	while(temp->next!=NULL){
		temp=temp->next;
	}
	temp->next=node;
	}
	return ;
	
}
void reverse(Node*&head)
    {
       
        Node* current = head;
        Node *prev = NULL, *next = NULL;
        while (current != NULL) {
            next = current->next;
            current->next = prev;
            prev = current;
            current = next;
        }
        head = prev;
    }
int main() {
	Node*head=NULL;
	int n,m;
	cin>>n>>m;
	Node*head1=NULL;
	Node*head2=NULL;
	for(int i=0;i<n;i++){
		int x;
		cin>>x;
		insertAtTail(head1,x);
	}
	for(int i=0;i<m;i++){
		int x;
		cin>>x;
		insertAtTail(head2,x);
	}
	reverse(head1);
	reverse(head2);
	Node*temp=NULL;
	int carry=0;
	int i=0;
	int j=0;
	Node*temp1=head1;
	Node*temp2=head2;
	while(i<n && j<m){
		int sum=temp1->data+temp2->data+carry;
		int append=sum%10;
		insertAtTail(temp,append);
		carry=sum/10;
		temp1=temp1->next;
		temp2=temp2->next;
		i++;
		j++;
	}
	while(i<n){
		int sum=temp1->data+carry;
		int append=sum%10;
		insertAtTail(temp,append);
		carry=sum/10;
		temp1=temp1->next;
		i++;
		
	}
	while(j<m){
	    int sum=temp2->data+carry;
		int append=sum%10;
		insertAtTail(temp,append);
		carry=sum/10;
		temp2=temp2->next;
		j++;
	}
	while(carry){
		insertAtTail(temp,carry%10);
		carry=carry/10;
	}
	reverse(temp);
	while(temp){
		cout<<temp->data<<" ";
		temp=temp->next;
	}

	return 0;
}
