Bug1
The incorrect original code or code snippit that you wrote:
cpp`````
//
//assignment10
//Question 7
#include <iostream>
#include <fstream>
#include <string>
using namespace std;
int main()
{
    string filename, line;
    int lines, counter = 0;
    cout << "Enter file name";
    cin >> filename;
    cout << "Enter an integer";
    cin >> lines;

    ifstream infile(filename);
    if (!infile)
    {
        cout << "NO file found" << endl;
        exit(1);
    }
    while (counter < lines && getline(infile, line)) {
        cout << line << "";
        counter++;
    }

    if counter < lines {
        cout << "File is displayed." << endl;
    }
    return 0;
}

`````````
What bug does the original code have?
Parenthesis is missing in the code in line 30

What misunderstanding of C++ concepts lead you to this incorrect code?

such mistakes can happen if the code is being written carelessly.

How to correct the bug?

we must check out our work once we are complete.

The corresponding bug-free code or code snippet is:
//`````
//assignment10
//Question 7
#include <iostream>
#include <fstream>
#include <string>
using namespace std;
int main()
{
    string filename, line;
    int lines, counter = 0;
    cout << "Enter file name";
    cin >> filename;
    cout << "Enter an integer";
    cin >> lines;

    ifstream infile(filename);
    if (!infile)
    {
        cout << "NO file found" << endl;
        exit(1);
    }
    while (counter < lines && getline(infile, line)) {
        cout << line << "";
        counter++;
    }

    if (counter < lines) {
        cout << "File is displayed." << endl;
    }
    return 0;
}

``````

What is the take-away message from this bug?
be carefull for the small small details too while writting the code.

Bug 2
The incorrect original code or code snippit that you wrote:

``````````````
//assignment10
//Question 7
#include <iostream>
#include <fstream>
#include <string>
using namespace std;
int main()
{
    string filename, line;
    int lines, counter = 0;
    cout << "Enter file name";
    cin >> filename;
    cout << "Enter an integer";
    cin >> lines;

    ifstream infile(filename);
    if (infile)
    {
        cout << "NO file found" << endl;
        exit(1);
    }
    while (counter < lines && getline(infile, line)) {
        cout << line << "";
        counter++;
    }

    if (counter < lines) {
        cout << "File is displayed." << endl;
    }
    return 0;
}

`````````

What bug does the original code have? 
line 107, ! is missing

What misunderstanding of C++ concepts lead you to this mistake? 
this misktake can sometimes happen due to carelessness.

How to correct the bug?
be carefull and check the code once you are done also read the questions carefully and always check the relative signs and puntuations 

The corresponding bug-free code or code snippet is:

``````
//assignment10
//Question 7
#include <iostream>
#include <fstream>
#include <string>
using namespace std;
int main()
{
    string filename, line;
    int lines, counter = 0;
    cout << "Enter file name";
    cin >> filename;
    cout << "Enter an integer";
    cin >> lines;

    ifstream infile(filename);
    if (!infile)
    {
        cout << "NO file found" << endl;
        exit(1);
    }
    while (counter < lines && getline(infile, line)) {
        cout << line << "";
        counter++;
    }

    if (counter < lines) {
        cout << "File is displayed." << endl;
    }
    return 0;
}

```````

What is the take-away message from this bug?
we should be carefull when we write the code.

Bug 3
The incorrect original code or code snippit that you wrote:

``````````````
//assignment10
//Question 7
#include <iostream>
#include <fstream>
#include <string>
using namespace std;
int main()
{
    string filename, line;
    int lines, counter = 0;
    cout << "Enter file name";
    cin >> filename;
    cout << "Enter an integer";
    cin >> lines;

    ifstream infile(filename);
    if (infile)
    {
        cout << "NO file found" << endl;
        exit();
    }
    while (counter < lines && getline(infile, line)) {
        cout << line << "";
        counter++;
    }

    if (counter < lines) {
        cout << "File is displayed." << endl;
    }
    return 0;
}

`````````

What bug does the original code have? 
NO value of exit is placed
What misunderstanding of C++ concepts lead you to this mistake? 
this misktake can sometimes happen due to carelessness.

How to correct the bug?
Enter the value as 1.
The corresponding bug-free code or code snippet is:

``````
//assignment10
//Question 7
#include <iostream>
#include <fstream>
#include <string>
using namespace std;
int main()
{
    string filename, line;
    int lines, counter = 0;
    cout << "Enter file name";
    cin >> filename;
    cout << "Enter an integer";
    cin >> lines;

    ifstream infile(filename);
    if (!infile)
    {
        cout << "NO file found" << endl;
        exit(1);
    }
    while (counter < lines && getline(infile, line)) {
        cout << line << "";
        counter++;
    }

    if (counter < lines) {
        cout << "File is displayed." << endl;
    }
    return 0;
}

```````

What is the take-away message from this bug?
we should be carefull when we write the code.
