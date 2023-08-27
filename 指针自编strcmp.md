# Start
#include<stdio.h>
int StrCmp(char* s1, char* s2)
{
	int i = 0;
	while (s1[i] == s2[i] && s1[i] != '\0' && s2[i] != '\0')
		i++;
	printf("%d", s1[i] - s2[i]);

}
int main()
{
	char n[100], m[100];
	scanf("%s%s",&m, &n);
	StrCmp(m,n);
	return 0;
}
