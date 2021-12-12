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
# Exercise Break - Good Morning, Good Afternoon, Good Evening, Good Night.
```
#include <iostream>
#include <string>
using namespace std;

string greetings(int time) {
    if (time < 11) { //the time (military time; 24hrs)
        return "Good Morning";
    }
    else if (time < 17) {
        return "Good Afternoon";
    }
    else if (time < 21) {
        return "Good Evening";
    }
    else if (time < 24) {
        return "Good Nighto"; //Oyasumi
    }
}
int main()
{
    cout << "What time is it?" << endl;//ask
    int userInput;
    cin >> userInput;//get user input
    cout << greetings(userInput) << endl;//result
    return 0;
}
```
