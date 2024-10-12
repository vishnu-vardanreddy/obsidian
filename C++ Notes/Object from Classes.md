```c++
#inlcud<iostream>
#define PI 3.14         // Macro define

int r = 2;             // Global Declaration
void display();      // function declaring globaly to use in out of the class
Class MyClass
{
	void display()
	{
		 std::cout<<"The journey starts from here"<<std::endl;
	}
};         // semicolen is musten
int main()
{
	MyClass m;
	m.display()
	std::cout<<"This is inside the main function"<<std::endl;
	m.area;
	int x =200;
	std::cout<<x<<std::endl;
}
int area()
{
	int a = PI*r*r;
	std::cout<<a<<std::endl;
}


```
for the above program instead of using the std:: all the time we can use the " using namespace std" which call all the components inside the namespace package.

# Constants
```c++
int main()
{
		const int x = 10; // the value is constant throughtout the programm.
}
```
To Work on strings
```c++
#include<string>
int main()
{
	std::string str = "Jay";
	std::cout<<str<<std::endl;
}
```

# Data Types in C++
- Primary datatype -> 
			int , float , double, char, wchar_t, bool, void
- Derived datatype ->
			Array, Pointer, Functions, Referance.
- User Defined ->
			Structure, Class, Union, Typeof

# note:
- The int type take only up to 10 digits to print if the number of digits excides it automatically throws the garbage value.
- The cout print only up to 6 digits. To print more numbers we need to use the "setprecession(1,2,3,19,.....)".
-  If we define the float value then it is preferred that use f at the end.
- To find the limits of the data types in c++ type "#include<limits.h>" and click ctrl+space.