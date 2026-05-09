#include <iostream>
using namespace std;
//inheritance

class Human
{
    //properties
    protected:
    string name;
};
class student: public Human
{
    int roll_no;
    
    public:
    student(string n, int a)
{
    name=n;
    roll_no=a;
}
void display()
{
    cout<<name<<" "<<roll_no<<endl;
}
};
int main()
{
    student obj("Divya", 20);
    obj.display();
}
