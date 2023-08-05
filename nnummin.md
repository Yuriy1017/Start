# Start
#include <stdio.h>

int main()
{
    int i,n,m,j,min,a;
    scanf("%d\n", &n);
    for (i=1;i<=n;i++)
    {  
        scanf("%d", &m);
        scanf("%d", &a);
        min = a;
        for (j = 2; j <= m; j++)
        {
            scanf("%d", &a);
            if (min > a)
                min = a;
        }
        printf("%d\n", min);
    }
    return 0;
}
