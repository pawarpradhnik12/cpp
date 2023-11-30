#include <iostream>
#include <fstream>
#include <cstring>
#include <vector>
using namespace std;
/*struct rec
{
    char *n;
    int a;
};*/

// Define a structure to store Name and Age
/*struct Person {
    char* name;
    int age;
};*/

// Define a structure to store Name and Age
struct Person {
    string name;
    int age;
};

int main()
{
    //part 1
    /*int n=100;
    struct rec rec[n];
    FILE *f;
    char name[20];
    int age;
    int i=0;
    char *temp;
    int k;
    int l;
    f=fopen("C:\\Users\\Aniketh Mehta\\Desktop\\myfile.csv","r");
    if(f==NULL)
    {
        cout<<"file open error!";
        exit(0);
    }
    cout<<"File opened successfully"<<endl;
    while(!feof(f))
    {
        fscanf(f,"%s,%d",name,&age);
        l=strlen(name);
        temp=(char*)malloc(l);
        strcpy(temp,name);
        rec[i].n=temp;
        rec[i].a=age;
        i++;
    }
    for(k=0;k<i;k++)
    {
        cout<<rec[k].n<<" "<<rec[k].a<<" "<<endl;
    }
    fclose(f);*/




    //part 2
    /*FILE *f;
    char name[20];
    int age;
    f=fopen("C:\\Users\\Aniketh Mehta\\Desktop\\myfile.csv","a");
    if(f==NULL)
    {
        cout<<"file open error!";
        exit(0);
    }
    for(int i=0;i<1;i++)
    {
        cout<<"Enter name:";
        cin>>name;
        cout<<"Enter age:";
        cin>>age;
        fprintf(f,"%s %d",name,age);
    }
    fclose(f);*/









    //part1_new
    /*const char* filename = "C:\\Users\\Aniketh Mehta\\Desktop\\myfile.csv";
    ifstream file(filename);

    if (!file) {
        cerr << "Failed to open file: " << filename << endl;
        return 1;
    }

    // Read the data from the CSV file
    vector<Person> people;
    string line;

    while (getline(file, line)) {
        char* cstr = new char[line.size() + 1];
        strcpy(cstr, line.c_str());

        // Parse the CSV line into Name and Age
        char* token = strtok(cstr, ",");
        if (token != nullptr) {
            Person person;
            person.name = new char[strlen(token) + 1];
            strcpy(person.name, token);

            token = strtok(nullptr, ",");
            if (token != nullptr) {
                person.age = atoi(token);
                people.push_back(person);
            } else {
                cerr << "Invalid CSV format in line: " << line << endl;
                delete[] person.name;
                delete[] cstr;
            }
        } else {
            cerr << "Invalid CSV format in line: " << line << endl;
            delete[] cstr;
        }
    }

    // Print the data
    for (const Person& person : people) {
        cout << "Name: " << person.name << ", Age: " << person.age << endl;
        delete[] person.name;
    }

    // Clean up allocated memory
    for (Person& person : people) {
        delete[] person.name;
    }*/


//part2_new
    /*const char* filename = "C:\\Users\\Mahenur Dalwale\\Desktop\\myfile.csv";

    ofstream file(filename, ios::app); // Open the file in append mode

    if (!file) {
        cerr << "Failed to open file: " << filename << endl;
        return 1;
    }

    Person person;
 // Input Name and Age
    cout << "Enter Name: ";
    cin >> person.name;

    cout << "Enter Age: ";
    cin >> person.age;

    // Write Name and Age to the file
    file << person.name << "," << person.age << endl;

    cout << "Data appended to " << filename << endl;*/
 return 0;

}
