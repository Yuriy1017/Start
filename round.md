# Start
int main()
{//辗转相除法，最大公约数
	int a, b;
	scanf("%d,%d", &a,&b);
	while (a != b&&a!=0&&b!=0)
		if (a > b)
			a = a % b;
		else
			b = b % a;
	printf("%d", (a>b?a:b));
	return 0;
}
