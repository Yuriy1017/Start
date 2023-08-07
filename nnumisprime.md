# Start
#include <math.h>
int main()
{//nnumisprime
	int n,f=1;
	while (scanf("%d", &n) != EOF)
	{
		if (n == 2)
		{
			printf("Yes\n");
			continue;
		}
		else if (n == 1)
		{
			printf("No\n");
			continue;
		}
		f = 1;
		for (int i = 2; i <= sqrt(n); i++)
			if (n % i == 0)
			{
				f = 0;
				break;
			}
		if (f == 1)
			printf("Yes\n");
		else
			printf("No\n");
	}

	return 0;
}
