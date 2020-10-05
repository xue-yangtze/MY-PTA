#include <stdio.h>

void pyramid( int n );

int main()
{    
    int n;

    scanf("%d", &n);
    pyramid(n);

    return 0;
}

/* 你的代码将被嵌在这里 */
void pyramid( int n ){
    int a,b,c,d;
    b=n-1;
    for(a=1;a<=n;a++){
        for(c=b;c>0;c--){
            putchar(' ');
        }
        for(d=a;d>0;d--){
            printf("%d ",a);
        }
        printf("\n");
        b--;
    }
}
