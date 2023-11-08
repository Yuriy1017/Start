# Start
#include<stdio.h>
void trans(int n, int base)
{
	char s[16] = "0123456789ABCDEF", c[20];
	int i = 0;
	while (n > 0)
	{
		c[i++] = s[n % base];
		n /= base;
	}
	for(int j=i-1;j>=0;j--)
	printf("%c", c[j]);
	printf("\n");
}
int main()
{
	int n;
	while (scanf("%d", &n) != EOF)
		trans(n, 2);
	return 0;
}
