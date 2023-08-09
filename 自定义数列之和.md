# Start
#include <stdio.h>
#include <math.h>
int main()
{
	float s,m,n;
	while (scanf("%f", &n) != EOF)
	{
		scanf("%f", &m);
		s = 0;
		for (int i=1;i<=m;i++)
		{
			s += n;
			n = sqrt(n);
		}
		printf("%.2f\n", s);
	}
	return 0;
}
