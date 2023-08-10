# Start
#include <stdio.h>

int main()
{
	int m, n,f=0 ;
	int arr[] = { 6, 28, 496, 8128, 33550336 };
	while (scanf("%d%d", &m, &n) != EOF & m != 0 &&n != 0)
	{
		f = 0;
		for (int j = 0; j < 5; j++)
		{
			
			if ((m <= arr[j]) && (arr[j] <= n))
			{
				if (f == 0)
					printf("%d", arr[j]);
				else
					printf(" %d", arr[j]);
				f = 1;
			}
			
		}
		if (f == 0)
			printf("No\n");
		else
			printf("\n");

	}
	return 0;
}
