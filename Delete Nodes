#include<bits/stdc++.h>
using namespace std;
class Node{
    public:
    int data;
    Node* next;
    Node(int d){
        data=d;
        next=NULL;
    }
};
void deletenodes(Node* &head){
    Node* curr=head;
    Node* maxnode=head;
    Node* temp;
    while(curr!=NULL && curr->next!=NULL){
            if(curr->next->data < maxnode->data){
                temp=curr->next;
                curr->next=temp->next;
                temp->next=NULL;
                delete temp;

            }
            else{
                curr=curr->next;
                maxnode=curr;
            }

    }
}
void reversell(Node* &head){
    Node* curr=head;
    Node* next=curr->next;
    Node* prev=NULL;
    while(curr!=NULL){
        next=curr->next;
        curr->next=prev;
        prev=curr;
        curr=next;

    }
    head=prev;
}
void insertAtTail(Node* &head,Node* &tail,int d){
    Node* temp=new Node(d);
    if(tail==NULL){
        tail=temp;
        head=temp;
        temp->next=NULL;
    }
    else{
        tail->next=temp;
        temp->next=NULL;
        tail=temp;
    }
}
void display(Node* &head){
    Node* temp=head;
    while(temp!=NULL){
        cout<<temp->data<<" ";
        temp=temp->next;
    }
    cout<<endl;
}
int main(){
    Node* head=NULL;
    Node* tail=NULL;
    int t;
    cin>>t;
    while(t--){
        int d;
        cin>>d;
        insertAtTail(head,tail,d);
    }
    reversell(head);
    deletenodes(head);
    reversell(head);
    display(head);
}
