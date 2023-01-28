# INSERTION-OPERATION-IN-ARRAY
Here in this repository i have shown that how elements are inserted in an array at any position through user input.PLEASE MARK THE STAR IF LIKED

#include<iostream>
#include<conio.h>
using namespace std;
class A
{
    public:
    void func()
    {
        int pos,ele,i;
        
        int arr[7]={1,2,3,4,5};
        int size=sizeof(arr)/sizeof(arr[0]);
        cout<<"the elements of the array are "<<endl;
        for(i=0;i<5;i++)
        cout<<arr[i]<<endl;
        cout<<"enter the elements-"<<endl;
        
        cin>>ele;
        cout<<"enter the position"<<endl;
        cin>>pos;
        size=size+1;
        for(i=size-1;i>=pos-1;i--)
        {
            arr[i+1]=arr[i];
            arr[pos-1]=ele;
            
        }
        for(i=0;i<size;i++)
        cout<<arr[i]<<endl;
    }
};
int main()
{
    A obj;
    obj.func();
    return 0;
}
                           
                           *CONCEPT
                           -declare the array of size n 
                           -print the elements to see the elements of the array
                           -take the input to get the element and the position from the user
                           -do size=size+1
                           -run a loop from size-1 to pos-1 because size is already size+1
                           -do arr[i+1]=arr[i] & arr[pos-1]=element taken from user
                           -run a loop again to print the array elements
                           
                           # PLEASE  GIVE ME A STAR IF LIKED
