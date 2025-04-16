# Linked lists

- implementing a linked list

```


#include "node.hpp"

class LinkedList {
private:
  node* head = nullptr;
  int length = =0; //for keeping track of list length

public: 
  void push_back(double value);
  void print() const; //used in assignment 5


};

---

node.hpp:

struct node {
  double value;
  node* next; //if not a pointer, would cause infinte recusion of making new nodes
};

linked_list.cpp

void LinkedList::push_back(double value)
{
  node* newNode = new node;
  new_node->value = value;
  new_node->next = nullptr;


  if(this->length == 0) {
    this->head = new newNode;
    this->length++;
    return;
}
  node* itr = this->head;
 // for (int i = 0; i < this->size; i++) {
 //   itr = itr->next;
 // }

  itr->next = new_node;
  this->length++;
}

void LinkedList::print() {
  node* itr = this->head;
  while (itr != nulltpr) {
    std::cout << itr->value << ", ";
    itr = itr->next; 
  }
    std::cout << itr->value;
}

int main()
{

}

```

# Recursion

a function that calls itself
