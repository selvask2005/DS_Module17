# Ex 5b Breadth First Graph
## DATE:21/4/25
## AIM:
To write a printQueue C function of the given graph that is to be traversed in the breadth first manner.

![image](https://github.com/user-attachments/assets/f483f48c-6af0-4027-a993-01c108a50933)


## Algorithm
1.Start
2.Start from the front index of the queue.
3.If the queue is empty, print "Queue is empty".
4.Otherwise, print "Queue contains" and display all items from front to rear.
5.Return after printing the queue contents.
6.End 

## Program:
```
/*
Program to traverse graph using BFS
Developed by: SELVA KUMAR A
RegisterNumber:  212222110042
*/

#include<stdio.h> #include <stdlib.h> #define SIZE 40

struct queue{ int items[SIZE]; int front;
intrear;
};
struct queue* createQueue();
voidenqueue(structqueue*q, int); int dequeue(struct queue* q); voiddisplay(struct queue* q); int isEmpty(struct queue* q); voidprintQueue(structqueue* q);

structnode{ int vertex;
struct node* next;
};

struct node*createNode(int);
struct Graph {
int numVertices; struct node**adjLists; int* visited;
};
voidprintQueue(structqueue*q){ int i=q->front; if(isEmpty(q))
{
printf("Queue is empty");
}
else
{
printf("Queue contains "); for(i=q->front;i<q->rear+1;i++)
{
printf("%d",q->items[i]);
}
}
}
```

## Output:

<img width="377" alt="image" src="https://github.com/user-attachments/assets/ef39ddf0-318d-4778-aedd-0945aee124e8" />


## Result:
Thus, the code for the printQueue function of the following graph that is to be traversed in the breadth first manner is implemented successfully.
