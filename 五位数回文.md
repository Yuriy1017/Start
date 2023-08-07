
#include <stdio.h>

int main()
{
    
	int s ;
	int i = 5;
	int arr[6] = { 0 };
	int a = 5;
	scanf("%d", &s);
	while (s>0)
	{
		arr[i] = s % 10;
		s = s /10;
		i--;
	}
	printf("%d\n", 5 - i);
	for (; i<a; a--)
		printf("%d",arr[a]);
	return 0;
}
