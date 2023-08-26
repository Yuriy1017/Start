# Start
#include<stdio.h>


int main()
{
	int n,lady=0,q=0,x=0,sum=0;
	char s[19],c[2];
	scanf("%d", &n);
	for (int i = 0; i < n; i++)
	{
		scanf("%s", &c);
		if (c[0] == 'q')
		{
			scanf("%d", &x);
			q++;
			sum += x;
		}
		else
		{
			scanf("%s", &s);
			if (s[16] % 2 == 0)lady++;

		}
	}
	
		printf("%d %d %d\n", n-q-lady,lady, sum/q);
	return 0;
}
