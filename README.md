# Repo
#include<iostream>
#include<cmath>
 
using namespace std;
 
int main()
{
    
    double num1,num2;
    char operation,redo;
    
    cout<<"WELCOME TO THE CALCULATOR PROGRAM:)"<<endl;
    cout<<"___________________________________"<<endl;
    cout<<endl<<endl<<endl;
   
    do
    {
       
        cout<<" Please enter an operation which you like to calculate (+,-,*,/)";
        cin>>operation ;
        cout<<endl<<endl;
        cout<<" Please enter two numbers to apply your requested operation(";
        cout<<operation<<"):"<<endl<<"1st num:";
        cin>>num1;
        cout<<"2nd num:" ;
        cin>>num2;
        cout<<endl;
        
        switch (operation)
        {
        
        case'+':
            cout<<"The addition of two numbers = ("<<num1<<","<<num2<<"):";
            cout<<num1+num2<<endl;
            break;
        case'-':
            cout<<"The substraction of two numbers ("<<num1<<","<<num2<<"):";
            cout<<num1-num2<<endl;
            break;
        case'*':
            cout<<"The multiplication of two numbers = ("<<num1<<","<<num2<<"):";
            cout<<num1*num2<<endl;
            break;
        case'/':
            cout<<"The division of two numbers = ("<<num1<<","<<num2<<"):";
            if(num2==0)
            {
                cout<<"not valid"<<endl;
            }
            cout<<(num1/num2)<<endl;
          
            break;
        default:
            cout<<"unknown command"<<endl;
 
        }
        //----now once again the program will ask the user if want to continue or not
        cout<<"enter y or Y to continue:";
        cin>>redo;
        cout<<endl<<endl;
    }
    while(redo=='y'||redo=='Y');
 
    return 0;
 
}
