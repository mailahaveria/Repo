# include <iostream>
using namespace std;

int main()
{
    char op, operation, redo;
    float num1, num2;

    cout << "Enter operator either + or - or * or /: ";
    cin >> op;
   

    cout <<endl<< "ENTER TWO OPERANDS: ";
 cout<<operation <<endl<<"1st num:";
        cin>>num1;
        cout<<"2nd num:" ;
        cin>>num2;
       

    switch(op)
    {
        case '+':
cout<<endl<<"ANSWER:"<<num1+num2<<endl;
          break;

        case '-':
            cout <<endl<<"ANSWER:"<< num1-num2;
            break;

        case '*':
            cout <<endl<< "ANSWER:"<<num1*num2;
            break;

        case '/':
            cout <<endl<<"ANSWER:"<< num1/num2;
            break;

        default:
            // If the operator is other than +, -, * or /, error message is shown
            cout << "Error! operator is not correct"<<endl;
           
           
    }
   

    return 0;
}

