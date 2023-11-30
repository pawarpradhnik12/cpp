#include <iostream>
using namespace std;

#define MAX_SIZE 5

class Queue {
private:
    int front, rear;
    int arr[MAX_SIZE];

public:
    Queue() : front(-1), rear(-1) {}

    bool isEmpty() {
        return front == -1 && rear == -1;
    }

    bool isFull() {
        return (rear + 1) % MAX_SIZE == front;
    }

    void enqueue(int value) {
        if (isFull()) {
            cout << "Queue is full. Cannot enqueue." << endl;
            return;
        }

        if (isEmpty()) {
            front = rear = 0;
        } else {
            rear = (rear + 1) % MAX_SIZE;
        }

        arr[rear] = value;
        cout << value << " enqueued to the queue." << endl;
    }

    void dequeue() {
        if (isEmpty()) {
            cout << "Queue is empty. Cannot dequeue." << endl;
            return;
        }

        cout << arr[front] << " dequeued from the queue." << endl;

        if (front == rear) {
            front = rear = -1;
        } else {
            front = (front + 1) % MAX_SIZE;
        }
    }

    void display() {
        if (isEmpty()) {
            cout << "Queue is empty." << endl;
            return;
        }

        cout << "Queue elements: ";
        int i = front;
        do {
            cout << arr[i] << " ";
            i = (i + 1) % MAX_SIZE;
        } while (i != (rear + 1) % MAX_SIZE);
        cout << endl;
    }

    void peek() {
        if (isEmpty()) {
            cout << "Queue is empty. Cannot peek." << endl;
            return;
        }

        cout << "Front element: " << arr[front] << endl;
    }
};

int main() {
    Queue queue;
    int choice, value;

    do {
        cout << "1. Enqueue\n";
        cout << "2. Dequeue\n";
        cout << "3. Display\n";
        cout << "4. Peek\n";
        cout << "5. Exit\n";
        cout << "Enter your choice: ";
        cin >> choice;

        switch (choice) {
            case 1:
                cout << "Enter value to enqueue: ";
                cin >> value;
                queue.enqueue(value);
                break;

            case 2:
                queue.dequeue();
                break;

            case 3:
                queue.display();
                break;

            case 4:
                queue.peek();
                break;

            case 5:
                cout << "Exiting the program." << endl;
                break;

            default:
                cout << "Invalid choice. Please try again." << endl;
        }
    } while (choice != 5);

    return 0;
}
