#include <stdio.h>
#include <stdlib.h>

char *digit_str[9]={"one","two","three","four","five","six","seven","eight","nine"};
char *two_digit_str[10]={"ten","eleven","twelve","thirteen","fourteen","fifteen","sixteen","seventeen","eighteen","nineteen"};
char *tens_str[8]={"twenty","thirty","forty","fifty","sixty","seventy","eighty","ninety"};

int main()
{
    //strings practical
    int n;
    printf("enter the five digit number:");
    scanf("%d",&n);
    //printf("%s",digit_str[n-1]);//one digit number



    /*if(n>9&&n<20)
    {
        printf("%s",two_digit_str[n-10]);//for example n=12
    }*/


    //two digit
    /*if(n>19&&n<=90)
    {
        int r=n%10;
        int q=n/10;
        //printf("%s %s",tens_str[q-2],digit_str[r-1]);
        printf("%s ",tens_str[q-2]);
        if(r!=0)
        {
            printf("%s",digit_str[r-1]);
        }
    }*/


    //three digit
    /*if(n>99&&n<1000)
    {
        int p=n/100;//n=359, 3=359/100
        printf("%s hundred ",digit_str[p-1]); //print three hundred
        int q=n%100;//n=359, 59=359%100
        int r=q/10;//5=59/10
        int s=q%10;//9=59%10
        //printf("%s %s",tens_str[r-2],digit_str[s-1]); //350 will give three hundred fifty null
        //printf("%s ",tens_str[r-2]);//print fifty
        if(r!=0)
        {
            printf("%s ",tens_str[r-2]);
        }
        if(s!=0)
        {
            printf("%s",digit_str[s-1]);//print nine
        }
    }*/


    //four digit
    /*if(n>999&&n<10000)
    {
        int p=n/1000;  //1=1234/1000;
        printf("%s thousand ",digit_str[p-1]);
        int q=n%1000; //234=1234%1000
        int r=q/100; // 2=234/100
        if(r!=0)
        {
            printf("%s hundred ",digit_str[r-1]);// for number 1000
        }
        int s=q%100; //34=234%100
        int t=s/10; //3=34/10
        int u=s%10; //4=34%10
        //printf("%s %s",tens_str[t-2],digit_str[u-1]);
        if(t!=0)
        {
            printf("%s ",tens_str[t-2]); //for number 1200
        }
        if(u!=0)
        {
            printf("%s",digit_str[u-1]); //for number 1230
        }
    }*/



    //five digit
    if(n>9999&&n<100000)
    {
        int p=n/10000; //1=12345/10000
        printf("%s thousand ",two_digit_str[p+1]);
        int q=n%1000; //345=12345%1000
        int r=q/100; //3=345/100
        if(r!=0)
        {
            printf("%s hundred ",digit_str[r-1]); //for number 12000
        }
        int s=q%100; //45=345%100
        int t=s/10; // 4=45/10
        int u=s%10; //5=45%10
        //printf("%s %s",tens_str[t-2],digit_str[u-1]);
        if(t!=0)
        {
             printf("%s ",tens_str[t-2]); //for number 12300
        }
        if(u!=0)
        {
            printf("%s",digit_str[u-1]);// for number 12340
        }
    }
    return 0;
}
