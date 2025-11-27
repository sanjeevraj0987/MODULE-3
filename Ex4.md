
# Ex.No:4
# Ex.Name: Write a C++ program to pass a password (Admin@123 )to the parameterized constructor of a base class through the derived class constructor.
## Date:21/08/25

## Aim:
To write a C++ program to pass a password (Admin@123 )to the parameterized constructor of a base class through the derived class constructor.

## Algorithm:
1. Start the program.
2. Define a base class with a string member to store a password.
3. Create a parameterized constructor in the base class to initialize the password.
4. Define a derived class that inherits from the base class.
5. In the derived class constructor, call the base class constructor and pass the password "Admin@123".
6. Provide a function in the base class to display the password.
7. In main(), create an object of the derived class.
8. Call the function to display the password.
9. End the program.

## Program:
```cpp
#include<iostream>
using namespace std;
 
class Parent {
    public:
    
    string pass="Admin@123";
    
    Parent(){
        cin>>pass;
        cout<<"The Password passed to the base class is "<<pass<<endl;
    }
     
    
};
 
class Child : public Parent
 {
     public:
     
     Child(){
         cout<<"The Password "<<pass<<" is passed through the derived class constructor"<<endl;
     }
 };
 int main()
 {
     Child obj;
 }
```

## Output:
<img width="1221" height="278" alt="Screenshot 2025-09-13 194258" src="https://github.com/user-attachments/assets/6394f063-61ef-448c-bedd-393ade699c2b" />

## Result:
The program successfully executed to pass a password (Admin@123 )to the parameterized constructor of a base class through the derived class constructor.
