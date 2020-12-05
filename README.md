#include <iostream>
using namespace std;
class Classroom
{
    char name[30];
    float age;
    public:
        void getdata(void);
        void putdata(void);
};
void Classroom ::getdata(void)
{
    cout<<"enter name:";
    cin>>name;
    cout<<"enter age:";
    cin>>age;
}
void Classroom::putdata(void)
{
    cout<<"Name: "<<name<<"\n";
    cout<<"Age: "<<age<<"\n";
}
const int size=3;
int main()
{
    Classroom student[size];
    for(int i=0;i<size;i++)
    {
        cout<<"\n the details of the student"<<i+1<<"\n";
        student[i].getdata();
        
    }
    cout<<"\n";
    for(int i=0;i<size;i++)
    {
        cout<<"\n Student"<<i+1<<"\n";
        student[1].putdata();
    }
    return 0;
}
