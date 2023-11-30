#include <iostream>
using namespace std;
class Date {
private:
    int day, month, year;

public:
    Date(int d, int m, int y) : day(d), month(m), year(y) {}

    void display() const {
        cout << day << "/" << month << "/" << year << endl;
    }

    // Function to check if a year is a leap year
    bool isLeapYear() const {
        if (year % 400 == 0 || (year % 4 == 0 && year % 100 != 0)) {
            return true;
        }
        return false;
    }

    // Function to get the number of days in a month
    int daysInMonth() const {
        if (month == 2) {
            return (isLeapYear() ? 29 : 28);
        } else if (month == 4 || month == 6 || month == 9 || month == 11) {
            return 30;
        } else {
            return 31;
        }
    }

    Date& operator++() {
        // Increment the day by 1
        day++;

        // Check for end of the month
        if (day > daysInMonth()) {
            day = 1;
            month++;
            if (month > 12) {
                month = 1;
                year++;
            }
        }

        return *this;
    }
};

int main() {
    Date today(18, 10, 2023);

    cout << "Today's date: ";
    today.display();

    // Increment the date by one day
    ++today;

    cout << "Tomorrow's date: ";
    today.display();

    return 0;
}
