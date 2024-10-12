To add comments the we use //-> for single line and for the multi line comments same as java or c.
We need to add header which consists of packages that are written with the "include" and then followed by package name in "<>".
In the header section itself we use the namespace concept. The namespace concept help to resolve the problem of calling the function with same names.
```c++
//Example:
#include<iostream
using namespace

namespace ns1
{
	int function()
	{
		--------------;
	}
}

namespace ns2
{
	void function()
	{
		--------------;
	}
}
```
Now from the above code if we want to call the function the compiler confuses with the same name in different namespaces so we use
```
ns1::function();
// for calling the function in the namespace1.
```
: : -> Scope Resolution operator.
