
#include <iostream>
using namespace std;

int main() {
    // Displaying the menu
    cout << "----- Calculator Menu -----" << endl;
    cout << "1. Add" << endl;
    cout << "2. Subtract" << endl;
    cout << "3. Multiply" << endl;
    cout << "4. Divide" << endl;
    cout << "5. Get Remainder" << endl;
    cout << "6. Exit" << endl;
    cout << "----------------------------------" << endl;

    // Getting user's choice
    int choice;
    cout << "Enter your choice (1-6): ";
    cin >> choice;

    // Variables to store user input
    double num1, num2;

    // Getting two numbers from the user
    cout << "Enter the first number: ";
    cin >> num1;
    cout << "Enter the second number: ";
    cin >> num2;

    // Perform the chosen operation
    float result;
    switch (choice) {
        case 1:
            result = num1 + num2;
            cout << "Result: " << result << endl;
            break;
        case 2:
            result = num1 - num2;
            cout << "Result: " << result << endl;
            break;
        case 3:
            result = num1 * num2;
            cout << "Result: " << result << endl;
            break;
        case 4:
            if (num2 != 0) {
                result = num1 / num2;
                cout << "Result: " << result << endl;
            } else {
                cout << "Error: Division by zero is not allowed." << endl;
            }
            break;
        /*case 5:
         float fmode;
            if (num2 != 0) {
                result = fmode(num1, num2); 
                cout << "Remainder: " <<  result << endl;
            } else {
                cout << "Error: Division by zero is not allowed." << endl;
            }
            break;*/
        case 6:
            cout << "Exiting the program. Goodbye!" << endl;
            break;
        default:
            cout << "Invalid choice." << endl;
    }

    return 0;
}
