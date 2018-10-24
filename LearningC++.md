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

We can have header file `PrintString.h`
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIwOTc5MjcyMTMsLTIwOTQ1Njc2MzQsLT
E2NzE4NzQ5MDUsLTY2ODg4ODIwMSwyNDAwMzQ2NSwtMTAzNTE4
MDk1MCwtMTI4MDMwMjE5MV19
-->