# Start
#include<string.h>
#include<stdio.h>

int main()
{
	int j, i, k; char n[10];
	while (scanf("%d%s", &k,&n) != EOF&&(k!=0||n[0]!=48))
	{
		for (i = 0; i < strlen(n); i++)
		{
			if (i != 0)printf(" ");
			switch (n[i])
			{
			case 49:for (j = 1; j <= k+2; j++)printf(" ");
				break;//1

			case 52:for (j = 1; j <= k+2; j++)printf(" ");
				break;//4

			default:printf(" ");
				for (j = 1; j <= k; j++)printf("-");
				printf(" ");
				break;
			}
		}
		printf("\n");
		for (i = 1; i <= k; i++)
		{
			for (int x = 0; x < strlen(n); x++)
			{
				if (x != 0)printf(" ");
				switch (n[x])
				{
				case 49:for (j = 1; j <= k + 1; j++)printf(" "); printf("|");
					break;//1
				case 50:for (j = 1; j <= k + 1; j++)printf(" "); printf("|");
					break;//2
				case 51:for (j = 1; j <= k + 1; j++)printf(" "); printf("|");
					break;//3
				case 55:for (j = 1; j <= k + 1; j++)printf(" "); printf("|");
					break;//7
				case 53:printf("|"); for (j = 1; j <= k + 1; j++)printf(" ");
					break;//5
				case 54:printf("|"); for (j = 1; j <= k + 1; j++)printf(" ");
					break;//6
				default:printf("|"); for (j = 1; j <= k; j++)printf(" "); printf("|");
					break;
				}
			}
			printf("\n");

		}
		for(i = 0; i < strlen(n); i++)
		{
			if (i != 0)printf(" ");
			switch (n[i])
			{
			case 48:for (j = 1; j <= k + 2; j++)printf(" ");
				break;//0
			case 49:for (j = 1; j <= k + 2; j++)printf(" ");
				break;//1

			case 55:for (j = 1; j <= k + 2; j++)printf(" ");
				break;//7

			default:printf(" ");
				for (j = 1; j <= k; j++)printf("-");
				printf(" ");
				break;
			}
		}
		printf("\n");
		for (i = 1; i <= k; i++)
		{
			for (int x = 0; x < strlen(n); x++)
			{
				if (x != 0)printf(" ");
				switch (n[x])
				{
				case 48:printf("|"); for (j = 1; j <= k; j++)printf(" "); printf("|");
					break;//0
				case 50:printf("|"); for (j = 1; j <= k + 1; j++)printf(" ");
					break;//2
				case 56:printf("|"); for (j = 1; j <= k; j++)printf(" "); printf("|");
					break;//8
				case 54:printf("|"); for (j = 1; j <= k; j++)printf(" "); printf("|");
					break;//6
				default:for (j = 1; j <= k + 1; j++)printf(" "); printf("|");
					break;
				}
			}
			printf("\n");
		}
		for (i = 0; i < strlen(n); i++)
		{
			if (i != 0)printf(" ");
			switch (n[i])
			{
			case 49:for (j = 1; j <= k + 2; j++)printf(" ");
				break;//1

			case 52:for (j = 1; j <= k + 2; j++)printf(" ");
				break;//4
			case 55:for (j = 1; j <= k + 2; j++)printf(" ");
				break;//7
			default:printf(" ");
				for (j = 1; j <= k; j++)printf("-");
				printf(" ");
				break;
			}
		}
		printf("\n");
		printf("\n");
	}
	return 0;
}
