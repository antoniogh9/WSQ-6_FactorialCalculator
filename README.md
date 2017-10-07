# WSQ-6_FactorialCalculator
This program basically asks the user for a non-negative value and then prints the factorial of it. Once it’s done the program asks if you would like to know the factorial of another number. If the user selects yes, then the program repeats. 
#include <iostream>
using namespace std ;
int main () {

int num, times, factorial ;
char ans ;

  do {
    times = 1 ;
    factorial = 1 ;

    cout << "Choose a non-negative number please: " ;
    cin >> num ;

    //Formula
    while (times <= num) {
      factorial = factorial * times ;
      ++times ;
    }

    cout << "The factorial of " << num << " is " ;
    cout << factorial << endl ;
    cout << "Would you like to try another number? [y/n]" << endl ;
    cin >> ans ;


  } while (ans == 'y') ;

    cout << "Have a nice day!" << endl ;

return 0;
}
