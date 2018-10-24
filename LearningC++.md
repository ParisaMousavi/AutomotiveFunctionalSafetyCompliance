# Learning C++

For programming with C++ we have some guidelines:
1. [A straightforward style guide](https://github.com/Microsoft/AirSim/blob/master/docs/coding_guidelines.md) 
2. [More detailed guidline](https://google.github.io/styleguide/cppguide.html)

First example for learning C++ is the following example
```python
 /*write a C++ program that outputs the following statement:
 *** "Hello world, I am ready for C++"
 */
 #include <iostream>

 int main() {
     std::cout << "Hello world, I am ready for C++";
     return 0;
 }
```

To avoid writting std:: we can use the following code snippets

```python
#include <iostream>
using namespace std;
int main()
{
    cout << "Hey, writing std:: is pain, ";
    cout << "change the program so I don't have to write it.";
    return 0;
}
```

** C++ functions**

```cpython
sizeof(int)
```
int 4
short 2
long 8
char 1
float 4
double 8
bool 1


**Constant**
```python
const int weightGoal = 100;
```

**For Loop**
```python
    for( int a = 1 ; a <= n ; a = a + 1){
        cout << str << endl;
    } 
```

We can have header file `PrintString.h`  as follows:
```python
#include <string>
void PrintString(std::string, int);
```

The header can be developed in `PrintString.cpp` file as follows:
```python
#include <iostream>
#include <string>
#include <PrintString.h>
using namespace std;
void PrintString(string str, int n)
{
    for( int a = 1 ; a <= n ; a = a + 1){
        cout << str << endl;
    } 
    for (int i = 0; i < n; i++) {
        cout << str << endl;
    }
}
```

And the developed function can be call in `main.cpp` as follows:
```python
#include <iostream>
#include <PrintString.h>
using namespace std;
int main()
{
    PrintString("This is a test.", 10);
}
```

**Example for Header and Recurcive function**


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIwMTE3Mjc4MSwtMTIyMDU4NDI2OCwtMj
A5NDU2NzYzNCwtMTY3MTg3NDkwNSwtNjY4ODg4MjAxLDI0MDAz
NDY1LC0xMDM1MTgwOTUwLC0xMjgwMzAyMTkxXX0=
-->