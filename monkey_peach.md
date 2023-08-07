# Start
#include <stdio.h>

int main()
{
	int n;
	long s = 0;
	while (scanf("%d", &n) != EOF)
	{
		s =1;
		for (int i = 1;i<n; i++)
				s = 2 * (s + 1);
		printf("%d\n",s);
	}
	return 0;
}
