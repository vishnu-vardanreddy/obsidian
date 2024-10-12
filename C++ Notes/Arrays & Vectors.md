Vector is a dynamic arrays which can change the size of the array. 
Note: Vector also stores only the same data type elements
```c++
#include<iostream>
#include<algorithm>
#include<vector>
using namespace std;
int main()
{
    vector<int> res ;
    vector<int> arr = {1,33,2,4,33};
    sort(arr.begin(), arr.end());
    for(int x : arr)
    {
        cout<<x<<" ";
    }
    cout<<endl;
    if(!arr.empty())
    {
        res.push_back(arr[0]);
    }
    for(int i = 1 ; i <arr.size() ; i++)
    {
        if(arr[i]!=arr[i+1])
        {
            res.push_back(arr[i]) ;
        }
    }
    cout<<endl;
    for(int x : res)
    {
        cout<<x<<" ";
    }
}
```

```c++
#include<iostream>
#inlcude<array>
using namespace std;
int main()
{
	array<int,3> arr = {1,2,3};
	for(auto x : arr)
	{
		cout<<x;
	}
}
```