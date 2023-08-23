# Start
#include <stdio.h>
int main()
{
	int arr[3999999] = { 1, 2, 3, 5, 8, 13, 21, 34, 55, 89};
	int n,m;
	scanf("%d", &n);
	for (int x=1;x<=n;x++)
	{
		int s=0,i=1;
		scanf("%d", &m);
		while (arr[i]<=m)
		{	
			if (arr[i] % 2 == 0)s += arr[i];
			i++;
			if (i > 9) arr[i] = arr[i - 1] + arr[i - 2];
		}
		printf("%d\n", s);

	}
	return 0;
}
