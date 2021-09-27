# Programs to convert from decimal to any other base in cpp.
## Decimal To Binary 
```cpp
#include <bits/stdc++.h>
using namespace std;
int decimalToBinary(int n)
{
    int ans = 0;
    int rem = 1;
    int i = 1;
    while (n != 0)
    {
        rem = n%2;
        n /= 2;
        ans = ans + rem * i ;
        i *= 10;
    }
    return ans ;

}
int main()
{

    int num;
    cout << "enter decimal number:- ";
    cin >> num;
    cout<< decimalToBinary(num);
}
```
## Decimal To Octal
```cpp
#include <bits/stdc++.h>
using namespace std;
int decimalToOctal(int n)
{
    int ans = 0;
    int rem = 1;
    int i = 1;
    while (n != 0)
    {
        rem = n%8;
        n /= 8;
        ans = ans + rem * i ;
        i *= 10;
    }
    return ans ;

}
int main()
{

    int num;
    cout << "enter decimal number:- ";
    cin >> num;
    cout<< decimalToOctal(num);
}
```
## Decimal To HexaDecimal
```cpp
#include <bits/stdc++.h>
using namespace std;
string decimalToHexadecimal(int n)
{
    int placevalue = 1;
    int ans = 0;
    int rem = 1;
    while (n != 0)
    {
        rem = n%2;
        n = n/2;
        if (rem <= 9)
        {
            ans = ans + rem * placevalue;
        }
        else
        {
            char c = 'A' + rem - 10;
        }
        placevalue *= 10;
    }
     
}
int main()
{

    int num;
    cout << "enter decimal number:- ";
    cin >> num;
    cout<< decimalToHexadecimal(num);
}
```

<h1 align="center"><i> keep learning keep exploring </i> </h1>
