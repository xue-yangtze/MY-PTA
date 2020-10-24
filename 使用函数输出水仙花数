#include <stdio.h>

int narcissistic( int number );
void PrintN( int m, int n );

int main()
{
    int m, n;

    scanf("%d %d", &m, &n);
    if ( narcissistic(m) ) printf("%d is a narcissistic number\n", m);
    PrintN(m, n);
    if ( narcissistic(n) ) printf("%d is a narcissistic number\n", n);

    return 0;
}

/* 你的代码将被嵌在这里 */
int narcissistic( int number ){
    int count=0;
    int num1=number;
    for(;num1!=0;){
        num1/=10;
        count++;
    }
    int n[count];
    int num2=number;
    for(int i=0;i<count;i++){
        n[i]=num2%10;
        num2/=10;
    }
    int j=1;
    int sum=0;
    for(int a=0;a<count;a++){
        int j=1;
        for(int b=0;b<count;b++){
            j*=n[a];
        }
        sum+=j;
    }
    int pd=0;
    if(sum==number){
        pd=1;
    }
    return pd;
}

void PrintN( int m, int n ){
    int i;
    for(i=m+1;i<n;i++){
        if(narcissistic( i)){
            printf("%d\n",i);
        }
    }
}
