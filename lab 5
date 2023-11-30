#include <iostream>
using namespace std;
int sum(int n);
int fact(int n);
void print_reverse_string(char *str);
void print_reverse_number(int i);
int main()
{
    int n,i;
    char str[20];
    cout<<"Enter a number:";
    cin>>n;
    cout<<"Addition of first n integers: "<<sum(n)<<endl;
    cout<<"Factorial of number is: "<<fact(n)<<endl;
    cout<<"Enter a string:";
    cin>>str;
    print_reverse_string(str);
    cout<<endl;
    cout<<"Enter a number:";
    cin>>i;
    print_reverse_number(i);
    return 0;
}

int sum(int n)
{
    if(n>0)
    {
        return (n+sum(n-1));
    }
    else
    {
        return 0;
    }
}

int fact(int n)
{
    if(n>1)
    {
        return (n*fact(n-1));
    }
    else
    {
        return 1;
    }
}

void print_reverse_string(char *str)
{
    if(*str!='\0')
    {
        print_reverse_string(str+1);
        cout<<*str;
    }
}

void print_reverse_number(int i)
{
    if(i>0)
    {
        cout<<(i%10);
        print_reverse_number(i/10);
    }
}
