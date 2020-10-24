#include <stdio.h>
#include <math.h>

int prime( int p );
int PrimeSum( int m, int n );

int main()
{
    int m, n, p;

    scanf("%d %d", &m, &n);
    printf("Sum of ( ");
    for( p=m; p<=n; p++ ) {
        if( prime(p) != 0 )
            printf("%d ", p);
    }
    printf(") = %d\n", PrimeSum(m, n));

    return 0;
}

/* 你的代码将被嵌在这里 */
int prime( int p ){
    int i,m=1;
    if(p<=1){
        m=0;
    }else{
        for(i=2;i<=sqrt(p);i++){
            if(p%i==0){
                m=0;
                break;
            }
        }
    }
    return m;
}

int PrimeSum( int m, int n ){
    int sum=0;
    int i,p;
    for(p=m;p<=n;p++){
        int a=1;
        if(p<=1){
            a=0;
        }else{
            for(i=2;i<=sqrt(p);i++){
                if(p%i==0){
                    a=0;
                    break;
                }
            }
        }
        if(a){
            sum+=p;
        }
    }
    return sum;
}
