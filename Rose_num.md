# Start
#include <stdio.h>

int main()
{
	int n,a,k=1;
	long s = 0;
	while (scanf("%d", &n) != EOF)
	{
		s = 0;
		k = n;
		for (int i = 1;i<=4; i++)
		{
			a =k%10;
			s += a*a*a*a;
			k /= 10;
		}
		if (s == n)
			printf("Yes\n");
		else
			printf("No\n");
	}
	return 0;
}
