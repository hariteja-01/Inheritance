#include <bits/stdc++.h>
using namespace std;
class student{
    private:
    int roll;
    protected:
    char section[10];
    public:
    void get(){
        cout << "enter roll no: ";
        cin >> roll;
    }
    void show(){
        cout << "your roll number is: " << roll << endl;
    }
};
class result : private student{
    private:
    float fees;
    public:
    void getdata(){
        get();
        cout << "enter fees: ";
        cin >> fees;
        cout << "enter section: ";
        cin >> section;
    }
    void display(){
        show();
        cout << "fees that you're paying: " << fees << endl;
        cout <<"section that you are in: "<< section << endl;
    }
};
int main(){
    result r;
    r.getdata();
    r.display();
    // r.get();
    // r.show();
    return 0;
}
