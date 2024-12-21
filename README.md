#include <iostream>
using namespace std;

// Function declarations
void sum();
void subruction();
void multipley();
void divide();

int main() {
    int n;
    cout << "Press 1 for addition" << endl;
    cout << "Press 2 for subtraction" << endl;
    cout << "Press 3 for division" << endl;
    cout << "Press 4 for multiplication" << endl;
    cin >> n; // Take input for the choice
    
    if (n == 1) {
        sum();
    } else if (n == 2) {
        subruction();
    } else if (n == 3) {
        divide();
    } else if (n == 4) {
        multipley();
    } else {
        cout << "Invalid option." << endl;
    }
    return 0;
}

// Function definitions
void sum() {
    int num1, num2;
    cout << "Enter the first number: ";
    cin >> num1;
    cout << "Enter the second number: ";
    cin >> num2;
    cout << "The sum is: " << num1 + num2 << endl;
}

void subruction() {
    int num1, num2;
    cout << "Enter the first number: ";
    cin >> num1;
    cout << "Enter the second number: ";
    cin >> num2;
    cout << "The subtraction is: " << num1 - num2 << endl;
}

void multipley() {
    int num1, num2;
    cout << "Enter the first number: ";
    cin >> num1;
    cout << "Enter the second number: ";
    cin >> num2;
    cout << "The multiplication is: " << num1 * num2 << endl;
}

void divide() {
    int num1, num2;
    cout << "Enter the first number: ";
    cin >> num1;
    cout << "Enter the second number: ";
    cin >> num2;
    if (num2 != 0) {
        cout << "The division result is: " << num1 / num2 << endl;
    } else {
        cout << "Error: Division by zero is not allowed." << endl;
    }
}