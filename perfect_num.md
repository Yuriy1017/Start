# Start
#include <stdio.h>

int main()
{
	int n, s=0;
	scanf("%d", &n);
	for (int i = 1; i < n; i++)
		if (n % i == 0)
			s += i;

	if (s==n)
		printf("%d is cloze.", n);
	else
		printf("%d is not cloze.", n);
	return 0;
}
