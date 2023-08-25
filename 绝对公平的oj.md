# Start
#include<stdio.h>
#include<string.h>
int main()
{
	char s[100];
	int n;
	scanf("%d", &n);
	for (int j = 1; j <= n; j++)
	{
		scanf("%s",&s);
			if (strcmp(s, "AC") == 0)printf("Accepted\n");
			else if (strcmp(s,"PE")==0)printf("Presentation Error\n");
			else if (strcmp(s, "WA") == 0)printf("Wrong Answer\n");
			else if (strcmp(s, "RE") == 0)printf("Runtime Error\n");
			else if (strcmp(s, "TLE") == 0)printf("Time Limit Exceeded\n");
			else if (strcmp(s, "MLE") == 0)printf("Memory Limit Exceeded\n");
			else if (strcmp(s, "OLE") == 0)printf("Output Limit Exceeded\n");
			else if (strcmp(s, "CE") == 0)printf("Compilation Error\n");
	}
	return 0;
}
