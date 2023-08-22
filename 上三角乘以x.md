# Start
#include <stdio.h>
int main()
{
	int n,m;
	int arr[10][10] = { 0 };
	while (scanf("%d%d", &n,&m) != EOF)
	{
		int f= 0, i, j;
		for (i = 0; i <= n - 1; i++)
			for (j = 0; j <= n - 1; j++)
			{
				scanf("%d", &arr[i][j]);
				arr[i][j] *= m;
			}

		for (i = 0; i <= n - 1; i++)
		{
			for (j = 0; j <= i-1; j++)
				arr[i][j]/=m;
		}
		for (i = 0; i <= n - 1; i++)
		{
			for (j = 0; j <= n - 1; j++)
				printf("%d ", arr[i][j]);
			printf("\n");
		}
	}
	return 0;
}
