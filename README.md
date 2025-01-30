# Assignment4_BTech2026_310

# Coding Questions : 30.01.25

OOPS:

Problem Statement:

Ques1:Bank Account Information

Platform Used:
Programiz

Approach:Encapsulation

Code1:

#include<iostream>
using namespace std;
class BankAccount
{
    long int account_no;
    int balance;
    public:
    BankAccount(int acc,int bal)
    {
         account_no=acc;
         balance=bal;
    }
    void getAccountNo(int);
    void getBalance(int);
    int setAccountNo();
    int setBalance();
    void deposit(int);
    void withdraw(int);
};
void BankAccount::getAccountNo(int acc_no)
{
    account_no=acc_no;
}
int BankAccount::setAccountNo()
{
    return account_no;
}
void BankAccount::getBalance(int bal)
{
    balance=bal;
}
int BankAccount::setBalance()
{
    return balance;
}
void BankAccount::deposit(int dep)
{
    balance=balance+dep;
}
void BankAccount::withdraw(int withdraw)
{
    balance=balance-withdraw;
}

int main()
{
  BankAccount B(12345,0);
  B.getAccountNo(123456798);
  cout<<"Account number :"<<B.setAccountNo()<<endl;
 B.getBalance(1000);
 cout<<"Balance :"<<B.setBalance()<<endl;
 B.deposit(1000);
 cout<<"Balance After Deposit :"<<B.setBalance()<<endl;
 B.withdraw(500);
 cout<<"Balance After withdraw :"<<B.setBalance()<<endl;
 return 0;
}

DBMS:

Platform Used:LeetCode

 Ques 1:Class having atleast 5 students

 Code 1:

# Write your MySQL query statement below
SELECT class
FROM Courses
group by class
having count(student)>4;

 DSA:

 
