/*
Name:Aniketh Mehta
PRN: 23070147002
*/
#include <iostream>
#include<cstring>
using namespace std;

/*void Swap(int &ra,int &rb)
{
    int temp;
    temp=ra;
    ra=rb;
    rb=temp;
}*/



//returning a function by reference
/*char& fun(char* str)
{
    return str[0];
}*/


/*void* operator new(size_t,size)
{
    int *p=(int*)malloc(sizeof(int)*5);
    cout<<"overloaded operator new.."<<endl;
    return p;
}*/

//define class
/*class student
{
    char name[50]="xyz";
    int prn=123;
 public:
  void disp_name()
     {
         cout<<name;
     }
  void input_data()
  {
      cout<<"enter your name:"<<endl;
      cin>>name;
      cout<<"enter your PRN:"<<endl;
      cin>>prn;
      cout<<"Hello "<<name<<" and PRN is "<<prn;
  }
};*/

class date
{
    int month_days[12]={31,28,31,30,31,30,31,31,30,31,30,31};
    char *months[12]={"Jan","Feb","Mar","Apr","May","Jun","Jul","Aug","Sept","Oct","Nov","Dec"};
    char *weekdays[7]={"Sun","Mon","Tue","Wed","Thur","Fri","Sat"};
    int day;
    int month;
    int year;
  public:
    void disp_date()
    {
        cout<<"Date is: "<<day<<"/"<<month<<"/"<<year<<endl;
    }
    void input_date()
    {
        cout<<"Enter day"<<endl;
        cin>>day;
        cout<<"Enter month"<<endl;
        cin>>month;
        cout<<"Enter year"<<endl;
        cin>>year;
    }
    bool is_leap()
    {
        if((year%4==0)&&(year%400==0))
        {
            cout<<year<<" year is leap"<<endl;
        }
        else
        {
            cout<<year<<" year is not leap"<<endl;
        }
    }
    /*int day_of_year()
    {
        int sum=0,sum1=0;
        for(int i=0;i<=11;i++)
        {
            sum=sum+month_days[i];
        }
        for(int j=8;j<=11;j++)
        {
            sum1=sum1+month_days[j];
        }
        cout<<"Total days from Jan 1 to Sept 11: "<<(sum-sum1)+11<<endl;
    }*/
    int day_of_year()
    {
        int sum=0;
        for(int i=0;i<=(month-2);i++)
        {
            sum=sum+month_days[i];
        }
        sum=sum+day;
        if((year%4==0)&&(year%400==0))
        {
            sum=sum+1;
        }
        cout<<"Total days from Jan 1 to today's date: "<<sum<<endl;
        return sum;
    }
    void disp_date1()
    {
        cout<<"Date without slashes: "<<day<<" "<<months[month-1]<<" "<<year<<endl;
    }
    void disp_weekday()
    {
        int n,days;
        //cout<<"Weekday for 11 Sept 2023: "<<weekdays[0]<<endl;
        cout<<"enter the number for weekday of Jan 1:"<<endl;
        cin>>n;
        days=day_of_year();
        int last=days%7;
        if(last==0)
        {
            int index1=(last+n)+6;
            cout<<"Weekday of today's date is: "<<weekdays[index1]<<endl;
        }
        else
        {
            int index2=(last+n)-1;
            cout<<"Weekday of today's date is: "<<weekdays[index2]<<endl;
        }

    }
    /*void findAge()
    {
        cout<<year-1999;
        int total_days=day_of_year();
    }
    void add_days()
    {

    }*/
public:
    date();
    date(int ,int ,int );
    void display();

};
date::date()
{

    day=0;
    month=0;
    year=0;
}
date::date(int d,int m, int y)
{
    day=d;
    month=m;
    year=y;
}
void date::display()
{
    cout<<"Date using constructor: "<<day<<" "<<month<<" "<<year<<endl;
}
int main()
{
    /*int a=10,b=20;
    Swap(a,b);
    cout<<a<<" "<<b<<endl;*/



    /*char s[20]="abc";
    char ch='A';
    fun(s)=ch;
    cout<<s<<endl;
    char ch1='B';
    fun(s)=ch1;
    cout<<s<<endl;*/



    /*//dynamic memory allocation
    int *p;
    int i;
    p=new int[5];
    cout<<"enter the 5 nos:"<<endl;
    for(i=0;i<5;i++)
    {
        cin>>p[i];
    }
    cout<<"elements are:"<<endl;
    for(i=0;i<5;i++)
    {
        cout<<p[i]<<endl;
    }
    delete []p;
    p=NULL;//no dangling pointer*/


    //overloaded operator new
    //int *p=new int[5];



     //lab started c++ 11/9/23
    //printing hello world
    //cout<<"Hello World!"<<endl;

    /*int i=5;
    float j=6.2;
    cout<<"i="<<i<<" and j="<<j<<endl;*/

    /*char name[50];
    int prn;
    cout<<"Enter name:";
    cin>>name;
    cout<<"Enter PRN:";
    cin>>prn;
    cout<<"Hello "<<name<<endl;
    cout<<"Your PRN is "<<prn<<endl;*/


    //student s;
    //cout<<s.name<<endl;
    //cout<<s.prn<<endl;
    //s.disp_name();
    //s.input_data();

    //class date
    date today;
    date dob(10,10,1999);
    today.input_date();
    today.disp_date();
    //today.is_leap();
    today.day_of_year();
    today.disp_date1();
    today.disp_weekday();
    dob.display();
    //today.findAge();



    //LAB8
    /*char str[20];
    char arr;
    char reverse_arr;
    cout<<"Enter a word:"<<endl;
    cin>>str;
    cout<<"Array is: ";
    for(int i=0;i<strnlen(str,20);i++)
    {
        cout<<str[i];
        arr=str[i];
    }
    cout<<endl;
    cout<<"Reverse of array is: ";
    for(int j=strnlen(str,20);j>=0;j--)
    {
        cout<<str[j];
        reverse_arr=str[j];
    }
    cout<<endl;
    if(arr==reverse_arr)
    {
        cout<<"word is palindrome";
    }
    else{
        cout<<"word is not a palindrome";
    }*/



    //length of string using pointer
    /*char *str="symbiosis";
    int len;
    for(int i=1;i<11;i++)
    {
        if(*str=='\0')
            break;
        *str++;
        len=i;
    }
    cout<<"length of string is: "<<len;*/

    return 0;
}
