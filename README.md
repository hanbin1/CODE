# CODE

//divide array

#include <stdio.h>




void divide(int *arr, int size, int final_D)
{
for(int i=0;i<size;i++)
{
arr[i]=arr[i]/final_D;
}
}

int main()
{
int n;
scanf("%d",&n);

int A[n];
for(int i=0;i<n;i++)
{scanf("%d",&A[i]);}

int q,d;
scanf("%d",&q);
long long int final_d=1;

while(q--)
{scanf("%d",&d);
final_d*=d;


}

if(final_d!=0)
{ 
divide(A,n,final_d);

for(int i=0;i<n;i++)
{
printf("%d ",A[i]);
}
}
else
{
for(int i=0;i<n;i++)
{A[i]=0;
printf("%d ",A[i]);
}
}
return 0;
}
