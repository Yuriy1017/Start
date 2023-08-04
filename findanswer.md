# Start
#include <stdio.h>
#include <math.h>

int main()
{
	float a, b, c;
	scanf("%f%f%f", &a, &b, &c);
	float d = b * b - 4 * a * c;
	if ((a == 0) && (b!=0))
		printf("%.6f", (-c) / b);
	else if (d < 0 || (a == 0 && b == 0))
		printf("No");
	else if (d == 0)
		printf("%.6f\n", (-b + sqrt(d)) / 2 / a);
	else
	{
		printf("%.6f\n", (-b + sqrt(d)) / 2 / a);
		printf("%.6f\n", (-b - sqrt(d)) / 2 / a);
	}

	return 0;
}
