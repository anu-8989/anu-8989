#include<iostream>
using namespace std;
class item{
    char name[30];
    int price;
public :
    void getdata();
    void putdata();
};
void item::getdata(){
    cout<<"enter the name"<<endl;
    cin>>name;
    cout<<"enter the price"<<endl;
    cin>>price;
}
void item::putdata(){
cout<<"name"<<" "<<name<<endl;
cout<<"price"<<" "<<price<<endl;
}
int main(){
    item it[3];
    int i,n;
    cin>>n;
    for (i=0;i<n;i++){
        it[i].getdata();
    }
    for(i=0;i<n;i++){
        it[i].putdata();
    }
    return 0;
}
