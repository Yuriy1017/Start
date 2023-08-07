# Start
#include <stdio.h>

int main()
{
	float n,k=0;
	double s = 0;
	while (scanf("%f", &n) != EOF)
	{
		k = 0;
		s = 0;
		for (int i = 1; i <= n; i++)
		{
			k +=i;
			s += 1 / k;
		}
		printf("%.4f\n", s);
	}
	return 0;
}
