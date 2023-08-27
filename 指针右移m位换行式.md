# Start
#include<malloc.h>
#include<stdio.h>
void  myAdjust(int* p, int  n, int  m)
{
	for (int i = n - m; i <= n - 1; i++)
		printf("%d\n", p[i]);
	for (int i = 0; i <= n - m - 1; i++)
		printf("%d\n", p[i]);
}
int main()
{
	int* p = NULL;
	int n, m;
	scanf("%d", &n);
	p = (int*)malloc(sizeof(int) * n);
	int arr[n];
	for (int i = 0; i < n; i++)
		scanf("%d", &arr[i]);
	scanf("%d", &m);
	myAdjust(arr, n, m);
	free(p);
	return 0;
}
