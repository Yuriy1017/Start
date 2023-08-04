# Start
#include <stdio.h>


int main()
{
	int arr[] = { 31,28,31,30,31,30,31,31,30,31,30,31 };
	int y, m, d, i;
	scanf("%d-%d-%d", &y, &m, &d);
	m--;
	for (i = 0; i < m; i++)
	{
		d += arr[i];
		if (i == 1)
			if (y % 400 == 0 || (y % 100 != 0 && y % 4 == 0))
				d++;
	}
	printf("%d", d);
	return 0;
}
