Aim:
To understand and demonstrate the different parameter passing techniques in C++:
1. Call by Value
2. Call by Reference using pointers
3. Call by Reference using reference variables
   
Apparatus:
- A computer with C++ compiler (like GCC, Turbo C++, Code::Blocks, or online IDEs)
- Basic understanding of functions and pointers in C++
- Text editor or IDE for writing the code

Program Explanations:

- Program 1: Call by Value

  Code Summary:
  A swap function is used to exchange the values of two variables. The values are passed **by value**, meaning a copy is made, and original variables remain unchanged.

  Observation:
  Swapped values are printed inside the function, but main still shows original values (3, 5).

- Program 2: Call by Reference using Pointers

  Code Summary:
  In this version, the `swap` function receives the addresses of the variables. It swaps the values **at those addresses**, directly affecting the original variables.

  Observation:
  Swapped values are printed inside and reflected in the main function (5, 3).

- Program 3: Call by Reference using Reference Variables

  Code Summary:
  This program shows how a single variable's value can be changed directly by passing it **by reference**. The variable is incremented by 48 inside the function.

  Observation:
  The value in main is updated to 51 after the function call.



Algorithm:

Program 1 – Call by Value:
1. Declare two integers `a = 3`, `b = 5`.
2. Pass them to the function `swap(a, b)`.
3. Inside the function, swap the values using a temporary variable.
4. Print swapped values inside the function.
5. Print original values in `main`.

Program 2 – Call by Reference using Pointers:
1. Declare two integers `a = 3`, `b = 5`.
2. Pass their addresses to `swap(&a, &b)`.
3. Inside the function, use pointers to swap values directly.
4. Print swapped values inside the function.
5. Print modified values in `main`.

Program 3 – Call by Reference using Reference Variable:
1. Declare an integer `a = 3`.
2. Pass it by reference to `swap(a)`.
3. Inside the function, increment the value by 48.
4. Print updated value inside the function.
5. Observe the change reflected in `main`.

Key Concepts:

- Call by Value: A copy of the actual variable is passed. Changes inside the function do not affect the original variable.

- Call by Reference (Pointers): The function receives the memory addresses of variables. Changes directly affect the original variables.

- Call by Reference (References): A reference alias is created. Any modification reflects directly on the original variable.

- Function Parameters: Way of passing data into functions. Critical for memory management and performance.

- Pointers and References: Core features in C++ that provide flexibility and control over memory.

Conclusion:
These three programs illustrate the differences between call by value and call by reference in C++.
- In call by value, the original data remains unchanged.
- In call by reference using pointers, and reference variables, changes are reflected in the original variables.
