# firstdemo
#include<stdio.h>
#include<string.h>
#include<stdlib.h>

struct Node
{
    int data;
struct Node *next;
struct Node *prev;
}*start,*newnode,*curr;
void create(int n);
void display();
void freelist();
  

int main()
{
    int n,c,node;
    int choice;
    int data;
    printf("1-create\n 2-display");
    printf("Enter your choice");
    scanf("%d",&choice);
    switch(choice)
    {
        case 1:
        printf("Enter the data");
        scanf("%d",&n);
        create(n);
        break;
        case 2:
        display();
        break;
    
    printf("Do you want continue press 1");
    scanf("%d",&c); 
    if(c==1)
    {
      freelist();
      break;
    }  
