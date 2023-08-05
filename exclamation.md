# Start
#include <stdio.h>


int main()
{
	int n,s=1;
	scanf("%d",&n);
	for (int i = 2; i <= n; i++)
		s *= i;
	printf("%d", s);
	return 0;
}
