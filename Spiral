#include<stdio.h>
#include<stdlib.h>
#include<time.h>

int main()
{
	srand(time(0));
	int *n = (int *)malloc(sizeof(int));
	*n=(rand()%10-1+1)+1;
	int **ar=(int **)malloc(*n*sizeof(int*));
	printf("Initially matrix is:\n");
	for(int i=0;i<*n;i++)
	{
		ar[i]=(int*)malloc(*n*sizeof(int));
		for(int j=0;j<*n;j++)
		{
			ar[i][j]=(rand()%100-1+1)+1;
			printf("%d ",ar[i][j]);

		}
		printf("\n");
	}
	printf("spiral matrix is:\n");
	int min=0,max=*n-1;
	while(min<=max)
	{
		int i=min,j=min;
		while(j<=max)
		{
			printf("%d ",ar[i][j]);
			j++;
		}
		j--,i++;
		while(i<=max)
		{
			printf("%d ",ar[i][j]);
			i++;
		}
		i--,j--;
		while(j>=min)
		{
			printf("%d ",ar[i][j]);
			j--;
		}
		j++;i--;
		while(i>min)
		{
			printf("%d ",ar[i][j]);
			i--;
		}
		min++,max--;
	}
	
	return 0;
}
