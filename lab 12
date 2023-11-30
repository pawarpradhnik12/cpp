#include <iostream>
using namespace std;

struct Node {
    int data;
    Node* next;
};

Node* head = nullptr;

void addNodeBeginning(int value) {
    Node* newNode = new Node;
    newNode->data = value;
    newNode->next = head;
    head = newNode;
}

void addNodeEnd(int value) {
    Node* newNode = new Node;
    newNode->data = value;
    newNode->next = nullptr;

    if (head == nullptr) {
        head = newNode;
        return;
    }

    Node* temp = head;
    while (temp->next != nullptr) {
        temp = temp->next;
    }
    temp->next = newNode;
}

void deleteNodeBeginning() {
    if (head == nullptr) {
        cout << "List is empty. Cannot delete from an empty list.\n";
        return;
    }

    Node* temp = head;
    head = head->next;
    delete temp;
}

void deleteNodeEnd() {
    if (head == nullptr) {
        cout << "List is empty. Cannot delete from an empty list.\n";
        return;
    }

    if (head->next == nullptr) {
        delete head;
        head = nullptr;
        return;
    }

    Node* temp = head;
    while (temp->next->next != nullptr) {
        temp = temp->next;
    }

    delete temp->next;
    temp->next = nullptr;
}

void displayList() {
    Node* temp = head;
    cout << "Linked List: ";
    while (temp != nullptr) {
        cout << temp->data << " -> ";
        temp = temp->next;
    }
    cout << "NULL\n";
}

int main() {
    int choice, value;

    do {
        cout << "\nMenu:\n";
        cout << "1. Add Node at the Beginning\n";
        cout << "2. Add Node at the End\n";
        cout << "3. Delete Node from the Beginning\n";
        cout << "4. Delete Node from the End\n";
        cout << "5. Display Linked List\n";
        cout << "6. Exit\n";

        cout << "Enter your choice: ";
        cin >> choice;

        switch (choice) {
            case 1:
                cout << "Enter the value to add at the beginning: ";
                cin >> value;
                addNodeBeginning(value);
                break;
            case 2:
                cout << "Enter the value to add at the end: ";
                cin >> value;
                addNodeEnd(value);
                break;
            case 3:
                deleteNodeBeginning();
                break;
            case 4:
                deleteNodeEnd();
                break;
            case 5:
                displayList();
                break;
            case 6:
                cout << "Exiting the program.\n";
                break;
            default:
                cout << "Invalid choice. Please enter a valid option.\n";
        }
    } while (choice != 6);

    return 0;
}
