#include<stdio.h>
#include<conio.h>
void main()
{
	int a[10],n,i,temp,j,p;
	printf("Enter the number of array elements: ");
	scanf("%d",&n);
	printf("Enter the elements: \n");
	for(i=0;i<n;i++)
	{
		scanf("%d",&a[i]);
	
	}	
	for(i=0;i<n-1;i++)
	{
		temp=a[i];
		for(j=i;j<n-1;j++)
		{
			
			if(temp>a[j+1])
			{
				p=j+1;
			}
		}
		temp=a[p];
		a[p]=a[i];
		a[i]=temp;

	}
	printf("Sorted array elements are :");
	for(i=0;i<n;i++)
	{
		printf("\n%d",a[i]);
	}
	
 	getch();
}
