#include <iostream>

using namespace std;



class person
{
    int age;
 public:
     person()
     {
         cout<<"Constructor base class"<<endl;
     }
};
class student:private person
{
    char name[20];
 public:
     student()
     {
         cout<<"Constructor derived class"<<endl;
     }
};
class employee:private person
{
    int id;
public:
    employee()
    {
        cout<<"Constructor derived class employee";
    }
};
int main()
{
    //person p;
    student s;
    employee e;
    return 0;
}
