# Start
#include <stdio.h>

int main()
{
    int i,n,m,j,max,a;
    scanf("%d\n", &n);
    for (i=1;i<=n;i++)
    {  
        scanf("%d", &m);
        scanf("%d", &a);
        max = a;
        for (j = 2; j <= m; j++)
        {
            scanf("%d", &a);
            if (max < a)
                max = a;
        }
        printf("%d\n", max);
    }
    return 0;
}
