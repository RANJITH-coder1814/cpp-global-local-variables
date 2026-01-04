# cpp-global-local-variables
C++ 
# C++ Variable Scope Demonstration

This repository contains a simple C++ program that demonstrates the concept of **global and local variables** and how variable scope affects program behavior.

## 📌 Program Overview
- A global variable is declared outside all functions.
- A local variable is declared inside a function.
- The program shows how:
  - Global variables retain their updated values across function calls.
  - Local variables exist only within the function where they are declared.

## 🧠 Concepts Covered
- Global variables
- Local variables
- Variable scope in C++
- Function execution and memory behavior

## 💻 Source Code
```cpp
#include<iostream>
using namespace std;

int g = 5;

void fun() {
    int a = 10;
    a++;
    g++;
    cout << a << " " << g << endl;
}

int main() {
    cout << g << endl;
    fun();
    cout << g << endl;
}
