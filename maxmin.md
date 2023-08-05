# Start
#include <stdio.h>


int main()
{
	int min,max,n,a;
	scanf("%d", &n);
	scanf("%d", &a);
	min = max = a;
	for (int i = 2; i <=n; i++)
	{
		scanf("%d", &a);
		if (min > a)
			min = a;
		else if (max < a)
			max = a;
	}
	
	printf("max=%d, min=%d", max,min);
	return 0;
}
