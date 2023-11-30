#include <iostream>
using namespace std;

const int MAX_SIZE = 100;

class Stack {
private:
    int top;
    int arr[MAX_SIZE];

public:
    Stack() {
        top = -1;
    }

    bool isFull() {
        return top == MAX_SIZE - 1;
    }

    bool isEmpty() {
        return top == -1;
    }

    void push(int data) {
        if (isFull()) {
            cout << "Stack Overflow. Cannot push element." << endl;
        } else {
            top++;
            arr[top] = data;
            cout << "Pushed " << data << " onto the stack." << endl;
        }
    }

    void pop() {
        if (isEmpty()) {
            cout << "Stack Underflow. Cannot pop element." << endl;
        } else {
            cout << "Popped " << arr[top] << " from the stack." << endl;
            top--;
        }
    }

    void display() {
        if (isEmpty()) {
            cout << "Stack is empty." << endl;
        } else {
            cout << "Stack elements: ";
            for (int i = 0; i <= top; i++) {
                cout << arr[i] << " ";
            }
            cout << endl;
        }
    }

    void peek() {
        if (isEmpty()) {
            cout << "Stack is empty. Cannot peek." << endl;
        } else {
            cout << "Top element: " << arr[top] << endl;
        }
    }
};

int main() {
    Stack stack;
    int choice, data;

    do {
        cout << "\nStack Menu:\n";
        cout << "1. Push\n";
        cout << "2. Pop\n";
        cout << "3. Display\n";
        cout << "4. Peek\n";
        cout << "5. Exit\n";
        cout << "Enter your choice: ";
        cin >> choice;

        switch (choice) {
            case 1:
                cout << "Enter data to push: ";
                cin >> data;
                stack.push(data);
                break;

            case 2:
                stack.pop();
                break;

            case 3:
                stack.display();
                break;

            case 4:
                stack.peek();
                break;

            case 5:
                cout << "Exiting the program.\n";
                break;

            default:
                cout << "Invalid choice. Please enter a valid option.\n";
        }
    } while (choice != 5);

    return 0;
}
