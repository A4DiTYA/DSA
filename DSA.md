#include <bits/stdc++.h>
using namespace std;
class Node{
public:
    int data;
     Node*next;
     
};
void linkedlist(Node *ptr){
    while( ptr!= NULL){
        cout<<ptr->data<<" ";
        ptr = ptr-> next;
    }
}


int main(){
    Node* head = new Node();
    Node* second = new Node();
    Node* third = new Node();
    Node* fourth = new Node();
// allocate memory for nodes in the linked list in heap
 head -> data =7;
 head -> next = second;

 second -> data =11;
 second -> next = third;

 third  -> data =41;
 third  -> next = fourth;

 fourth -> data =66;
 fourth -> next = NULL;
linkedlist(head);
 return 0;
}
// traversal through a linked list
