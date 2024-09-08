- 👋 Hi, I’m @Erlaansaatpev
#include <iostream>
using namespace std;

int main() {
    double num1, num2;
    char operation;

    cout << "Введите первое число: ";
    cin >> num1;

    cout << "Введите операцию (+, -, *, /): ";
    cin >> operation;

    cout << "Введите второе число: ";
    cin >> num2;

    switch (operation) {
        case '+':
            cout << "Результат: " << num1 + num2 << endl;
            break;
        case '-':
            cout << "Результат: " << num1 - num2 << endl;
            break;
        case '*':
            cout << "Результат: " << num1 * num2 << endl;
            break;
        case '/':
            if (num2 != 0)
                cout << "Результат: " << num1 / num2 << endl;
            else
                cout << "Ошибка: деление на ноль!" << endl;
            break;
        default:
            cout << "Неверная операция!" << endl;
            break;
    }

    return 0;
}
