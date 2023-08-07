# Start
#include <stdio.h>
#输入的值越小就越精确
int main()
{
	float n,k=0;
	int f;
	double s = 0;
	while (scanf("%f", &n) != EOF)
	{
		s = 0;
		f = -1;
		for (int i = 1;1; i++)
		{
			k =2*i-1;
			f *= -1;
			s += 1 / k*f;
			if (1 / k <  n)
				break;
		}
		printf("%.4f\n", s*4);
	}
	return 0;
}
