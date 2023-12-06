# Start
#include <stdio.h> 
void main() 
{
	int n, m,x, t,i,op;
	int a[20], b[20][2];
	scanf("%d%d", &n, &m);
	for (i = 0; i < n; i++)
		scanf("%d", &a[i]);
	for (i = 0; i < m; i++)
		scanf("%d%d", &b[i][0], &b[i][1]);
	scanf("%d", &t);
	for (i = 0; i < t; i++)
	{
		scanf("%d", &op);
		if (op == 1)
		{
			scanf("%d", &x);
			int p = b[x-1][0];
			int q = b[p-1][1];
			printf("%d\n",a[q-1]);
		}
		else
		{
			scanf("%d", &x);
			scanf("%d%d", &b[x-1][0], &b[x-1][1]);
		}

	}
}
