# Patterns 
- 0-1 Pattern 
```cpp
// print 0-1 patten
/*
1
0 1        
1 0 1      
0 1 0 1    
1 0 1 0 1 
*/
#include<iostream>
using std::cout;
using std::cin;
using std::endl;

int main()
{
    int n,i,j,sum;
    cout<<"Enter number of rows:-";
    cin>>n;

    for (i = 1; i <= n; i++)
    {
        for (j = 1; j<= i; j++)
        {
            if ((i+j)%2 == 0)
            {
               cout<<"1"<<" ";
            }
            else{
                cout<<"0"<<" ";
            }
        }
        cout<<endl;
        
    }
    
}
```
- Floyd's Triangle
```cpp
// Print Floyd's Triangle
// 1
// 2 3
// 4 5 6
// 7 8 9 10
// 11 12 13 14 15

#include <iostream>
using namespace std;
int main()
{
    int n;
    cout << "enter a number of rows :- ";
    cin >> n;
    int num = 1;
    for (int i = 1; i <= n; i++)
     {
         for (int j = 1; j <= i; j++)
         {
            cout<<num<<" ";
            num++;
         }
         cout<<endl;
     }
}
```
-  Half Pyramid after 180 degree rotation
 ```cpp
//      *
//     **
//    ***
//   ****
//  *****
// ******
#include <iostream>
using namespace std;
int main()
{
    int n;
    cout << "enter a number of rows :- ";
    cin >> n;

    for (int i = 1; i <= n; i++)
    {
        for (int j = 1; j <= n; j++)
        {
            if (j <= n - i)
            {
                cout << " ";
            }
            else
            {
                cout << "*";
            }
        }
        cout << endl;
    }
}
```
- Half Pyramid using numbers
```cpp
// 1 
// 1 2 
// 1 2 3 
// 1 2 3 4 
// 1 2 3 4 5 
#include <iostream>
using namespace std;
int main()
{
    int n;
    cout << "enter a number of rows :- ";
    cin >> n;
    for (int i = 1; i <= n; i++)
     {
         for (int j = 1; j <= i; j++)
         {
            cout<<j<<" ";
         }
         cout<<endl;
     }
}
```
- Inverted Half Pyramid
```cpp
// Print an Inverted Half pyramid
// * * * * *  
// * * * *
// * * *
// * *
// *
#include<iostream>
using namespace std;
int main(){
    int n;
    cout<<"enter a number of rows :- ";
    cin>>n;
    for (int i = n; i >= 1; i--)
    {
        for (int j = 1; j <= i ;j++)
        {
            /* code */
            cout<<"*"<<" ";
            
        }
        cout<<" "<<endl;
    }
    
}   
```
- Half Pyramid using numbers - 
```cpp
// 1
// 2 2
// 3 3 3
// 4 4 4 4
// 5 5 5 5 5
// 6 6 6 6 6 6
// 7 7 7 7 7 7 7
#include <iostream>
using namespace std;
int main()
{
    int n;
    cout << "enter a number of rows :- ";
    cin >> n;
    for (int i = 1; i <= n; i++)
     {
         for (int j = 1; j <= i; j++)
         {
            cout<<i<<" ";
         }
         cout<<endl;
     }
}
```
- Inverted Half Pyramid using numbers
```cpp
// 1 2 3 4 5  
// 1 2 3 4
// 1 2 3
// 1 2
// 1
#include<iostream>
using namespace std;
int main(){
    int n;
    cout<<"enter a number of rows :- ";
    cin>>n;
    for (int i = n; i >= 1; i--)
    {
        for (int j = 1; j <= i ;j++)
        {
            /* code */
            cout<<j<<" ";
        }
        cout<<" "<<endl;
    }
    
} 
```
- Triangle patten
```cpp
//         *
//        * *
//       * * *
//      * * * *
//     * * * * *
//    * * * * * *
//   * * * * * * *
//  * * * * * * * *
// * * * * * * * * *
#include <iostream>
using namespace std;
int main()
{
    int n;
    cout << "enter a number of rows :- ";
    cin >> n;
    for (int i = 1; i <= n; i++)
    {
        for (int j = 1; j <= n; j++)
        {
            /* code */
            if (j <= n - i)
            {
                /* code */
                cout << " ";
            }
            else
            {
                cout << "* ";
            }
        }
        cout << endl;
    }
}
```
- Triangle of Numbers
```cpp
/*       1     
        1 2    
       1 2 3   
      1 2 3 4  
     1 2 3 4 5
*/ 
#include <iostream>
using namespace std;
int main()
{
    int n;
    cout << "enter a number of rows :- ";
    cin >> n;
    for (int i = 1; i <= n; i++)
    {
        for (int j = 1; j <= n-i; j++)
        {
           cout<<" ";
        }
        for (int j = 1; j<= i; j++)
        {
            cout<<j<<" ";
        }
        
        cout << endl;
    }
}
```
- Butterfly Pattern
```cpp
/*
*        *
**      **
***    ***
****  ****
**********
**********
****  ****
***    ***
**      **
*        *
*/
#include <iostream>
using namespace std;
int main(){
    int n;
    cout<<"no of rows:- ";
    cin>>n;

    for (int i = 1; i <= n; i++)
    {
        for (int j = 1; j <= i; j++)
        {
            cout<<"*";
        }
        for (int j = 1; j <= 2*n-2*i; j++)
        {
            cout<<" ";
        }
        for (int j = 1; j <= i; j++)
        {
            cout<<"*";
        }
        cout<<endl;
    }
    for (int i = n; i >= 1; i--)
    {
        for (int j = 1; j <= i; j++)
        {
            cout<<"*";
        }
        for (int j = 1; j <= 2*n-2*i; j++)
        {
            cout<<" ";
        }
        for (int j = 1; j <= i; j++)
        {
            cout<<"*";
        }
        cout<<endl;
    }
    
}
```
