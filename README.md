//Singly linked list;simple program 
#include<stdio.h>
#include<conio.h>
#include<stdlib.h>
struct  Sll
	{
		
		int info;
		Sll *next;
		
	};
	int main()
	{
		Sll *first,*second,*third,*forth;
			forth= (struct Sll*)malloc(sizeof(struct Sll));
		forth->info=8;
		forth->next=NULL;
		third= (struct Sll*)malloc(sizeof(struct Sll));
			third->info=6;
			third->next=forth;
			second= (struct Sll*)malloc(sizeof(struct Sll));
		second->info=4;
		second->next=third;
		first= (struct Sll*)malloc(sizeof(struct Sll));
			first->info=2;
			first->next=second;
	
		
	
		Sll *p=first;
		while(p!=NULL){
			printf("%d\t",p->info);
			p=p->next;
		}
	return(0);
	getch();	
	}
