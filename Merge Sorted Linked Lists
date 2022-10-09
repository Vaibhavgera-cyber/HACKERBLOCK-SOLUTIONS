#include<iostream>
using namespace std;

class node{
public:
	int data;
	node*next;
	node(int d){
		data=d;
		next=NULL;
	}
};
void insertAtTail(node*&head,int data){
	if(head==NULL){
		head=new node(data);
		return ;
	}
	node*tail=head;
	while(tail->next!=NULL){
		tail=tail->next;

	}
	node*n=new node(data);
	tail->next=n;

}
void buildList(node* &head){
	int n;
	cin>>n;
	while(n--){
		int data;
		cin>>data;
		insertAtTail(head,data);
	}
}
node *merge(node* &a,node* &b){
	if(a==NULL){
		return b;
	}
	if(b==NULL){
		return a;
	}
	node*c;
	if(a->data<b->data){
		c=a;
		c->next=merge(a->next,b);
	}
	else{
		c=b;
		c->next=merge(a,b->next);
	}
	return c;
}
void print(node*head){
	while(head!=NULL){
		cout<<head->data<<" ";
		head=head->next;
	}
	cout<<endl;
}
istream& operator>>(istream& is,node* &head){
	buildList(head);
return is;
}
ostream& operator<<(ostream &os,node* &head){
	print(head);
	return os;
}

int main(){
	int t;
    cin>>t;
    while(t--){
        node *head=NULL;
        node*head_2=NULL;
        cin>>head;
        
        cin>>head_2;
        node*a=head;
        node*b=head_2;
        node*newHead=merge(a,b);
        cout<<newHead;
    }
	
	return 0;
}
