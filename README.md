# Asks the user to enter a number then print its cube and square root. (EXERCISE 1)
```
#include <iostream>
#include <math.h>
using namespace std;

int main()
{
    double x;
    cout << "Input number \n";
    cin >> x;
    while (cin.fail())
    {
        cin.clear();
        cin.ignore();
        cout << "Invalid number please enter A NUMBER \n";
        cin >> x;
    }
    cout << "square root is " << sqrt(x) << endl;
    cout << "cube root is " << cbrt(x) << endl;
}
```
# 
