#include <iostream>

using namespace std;

int main() {
    // Устанавливаем корректное отображение символов (опционально для Windows)
    setlocale(LC_ALL, "Russian");

    double num1, num2;
    char op;

    cout << "--- Простой калькулятор ---" << endl;
    cout << "Введите первое число: ";
    cin >> num1;

    cout << "Введите оператор (+, -, *, /): ";
    cin >> op;

    cout << "Введите второе число: ";
   cin >> num2;

  cout << "Результат: ";

  switch (op) {
        case '+':
            cout << num1 + num2;
            break;
        case '-':
            cout << num1 - num2;
            break;
        case '*':
            cout << num1 * num2;
            break;
        case '/':
            if (num2 != 0) {
                cout << num1 / num2;
            } else {
                cout << "Ошибка! Деление на ноль невозможно.";
            }
            break;
        default:
            cout << "Ошибка! Неверный оператор.";
    }

  out << endl;
    return 0;
}
