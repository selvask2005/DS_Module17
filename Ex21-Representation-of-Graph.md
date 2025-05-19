# Ex 5A Representation of Graph
## DATE:21/04/25
## AIM:
To write a C program to display the adjacency matrix of the given graph by supplying the edges and the number of vertices.

## Algorithm
1.Start
2.Read the value of V (number of vertices).
3.Declare an adjacency matrix adjMatrix[V][V].
4.Initialize the matrix to 0 using the init function.
5.Calculate the maximum number of edges me as n * (n - 1) / 2.
6.For each edge, read e1 and e2, add the edge to the adjacency matrix, and stop if e1 == -1 && e2 == -1.
7.Print the adjacency matrix.
8.End

## Program:
```
/*
Program to display the adjacency matrix of the given graph
Developed by: Beatrice Thomas
RegisterNumber:  212223110005
*/
/*#include<stdio.h> int V;

//init matrix to 0 voidinit(int arr[][V])
{
int i,j;
for(i = 0; i < V; i++) for(j= 0; j< V; j++)
arr[i][j] = 0;
}
*/
int main()
{ int e1,e2,me,n,i;
scanf("%d",&V); int adjMatrix[V][V]; init(adjMatrix); n=V;
me=n*(n-1)/2; for(i=0;i<me;i++)
{
scanf("%d%d",&e1,&e2); addEdge(adjMatrix,e1,e2); if(e1==-1 && e2==-1)
{
break;
}
}
printAdjMatrix(adjMatrix);
}
```

## Output:

<img width="298" alt="image" src="https://github.com/user-attachments/assets/a28ec259-70b4-431c-8749-c9191850332b" />



## Result:
Thus, the C program to print the adjacency matrix of the given graph is implemented successfully.
