# Start
#include <stdio.h>
int main()
{//nnumaverage
    int i,n,m,j;
    float a,s;
    scanf("%d\n", &n);
    for (i=1;i<=n;i++)
    {  
        scanf("%d", &m);
        s = 0;
        for (j = 1; j <= m; j++)
        {
            scanf("%f", &a);
            s += a;
        }
        
        printf("%.2f\n", s/m);
    }
    return 0;
}
