# Start
#include <stdio.h>
#include <math.h>
int main()
{
	int m, n, s = 0, f = 0;;
	
	while (scanf("%d", &m) != 0)
	{
		scanf("%d", &n);
		for (int j = (m > 2 ? m : 2); j <= n; j++)
		{
			s = 0;
			for (int i = 1; i < j; i++)
				if (j % i == 0)
					s += i;

			if (s == j)
			{
				printf("%d ", s);
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
