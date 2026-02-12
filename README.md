# Dynamic Matrix Analyzer (Pointer Arithmetic)

This C++ program is a sophisticated tool for processing matrices of arbitrary sizes. Unlike standard array indexing, this implementation uses **dynamic memory allocation** and **direct pointer arithmetic** to manage and traverse data.

###  Mathematical & Technical Logic
The program flattens a 2D matrix structure into a contiguous 1D block of memory. To access an element at row $i$ and column $j$, it utilizes the row-major mapping formula:
$$\text{Address} = \text{BasePointer} + (i \times \text{columns} + j)$$



By using `*(matrix + i * cols + j)`, the application bypasses high-level syntax to interact directly with memory addresses, demonstrating a deep understanding of C++ memory models.

This project was developed as part of the programming curriculum at **Lviv Polytechnic National University**.

###  Key Features
* **Dynamic Sizing:** Allows users to define matrix dimensions (`rows` x `cols`) at runtime, utilizing the heap via the `new[]` operator.
* **Pointer Arithmetic:** Uses address-based access for both input and output, showing low-level programming proficiency.
* **Extrema Search:** Efficiently identifies the maximum and minimum values along with their original 2D coordinates.
* **Memory Safety:** Includes explicit deallocation using `delete[]` to ensure no memory leaks occur during execution.

###  Technical Stack
* **Language:** C++
* **Concepts:** Pointers, Dynamic Memory Management, Address Arithmetic, 2D-to-1D Mapping.

###  How to Use
1. Compile the code using a C++ compiler (e.g., GCC or Clang).
2. Enter the number of rows and columns.
3. Input the matrix elements.
4. The program will display the matrix and provide the values and positions of the Max and Min elements.
