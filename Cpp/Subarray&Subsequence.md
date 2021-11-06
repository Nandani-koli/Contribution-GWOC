# Subarray 
*A Subarray is defined as a continous part of a given array.*

***Example->***

Given Array :- 
|1|5|7|3|9|
|---|---|---|---|---|
 
*Following are the possible subarrays of given array ->*

`1`&nbsp;&nbsp;`1 5`&nbsp;&nbsp;`1 5 7 ` &nbsp;&nbsp;`1 5 7 3 `&nbsp;&nbsp;`1 5 7 3 9 `&nbsp;&nbsp;`5`&nbsp;&nbsp;`5 7`&nbsp;&nbsp; `5 7 3 `&nbsp;&nbsp;`5 7 3 9`&nbsp;&nbsp; `7 `&nbsp;&nbsp;`7 3 `&nbsp;&nbsp;`7 3 9`&nbsp;&nbsp; `3 `&nbsp;&nbsp;`3 9 `&nbsp;&nbsp;`9 `

Formula to find number of subarray with n elements :- n*(n+1)/2

## Program to print Subarray
```cpp
#include <iostream>
using namespace std;
int main()
{
    int n;
    cout<<"Enter size of array:-";
    cin>>n;
    int a[n];
    cout<<"Enter array elements:-";
    for(int i = 0; i <n;i++)
    {
        cin>>a[i];
    }
    
    for(int i = 0; i<n; i++)
    {
        for(int j=i;j<n; j++)
        {
            for(int k = i; k<=j; k++)
            {
                cout<<a[k]<<" ";
            }
            cout<<endl;
        }
    }
}
```
## Output :-
![Subarray](https://user-images.githubusercontent.com/70843941/140601332-79d716b9-1910-4d1a-9117-1c1dd0388c73.png)

# Subsequence
*A subsequence is defined as a sequence that can be derived from an array by selecting zero or more elements without changing the order of the remaining elements.*

***Example->***

Given Array :- 
|1|5|7|3|9|
|---|---|---|---|---|

*Following are the possible subsequence of given array ->*

