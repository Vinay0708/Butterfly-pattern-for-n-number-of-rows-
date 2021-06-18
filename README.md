# Butterfly-pattern-for-n-number-of-rows-
#include <stdio.h>
int main()
{   
    int star,space,row,x,n;
    printf("Entr the number of rows:");
    scanf("%d",&n);
    x=2*n-2;
    for(row=1;row<=n;row++)
    {
        for(star=1;star<=row;star++)
           printf("*");
        for(space=1;space<=x;space++)
           printf(" ");
        for(star=1;star<=row;star++)
           printf("*");
        x=x-2;
        printf("\n");
    }
    x=0;
    for(row=1;row<=n;row++)
    {
        for(star=1;star<=n+1-row;star++)
            printf("*");
        for(space=1;space<=x;space++)
            printf(" ");
        for(star=1;star<=n+1-row;star++)
            printf("*");
        x=x+2;
        printf("\n");
    }
   
    return 0;
}
