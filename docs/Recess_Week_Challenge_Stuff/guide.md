# Recess Week Challenge Hackerrank Guide

Typically, the first line of the question specifies the parameters for the input, such as the number of lines, values of variables. It is usually followed by a specified number of lines containing data separated by spaces.

Input Example (2 represents the number of lines to be followed by $(x)$, 1 8 3 is one line of data (to be read into first line of list), 4 5 6 is the second line of data (to be read into second line of list))
```bash
2
1 8 3
4 5 6
```

Output Example
```bash
1 2 3
```

## Python3 Guide

To read the first line of input,

```python
x = int(input()) # The int() is used to convert input from a string to integer
```

To read the subsequent 2 lines of input
```python
my_list = []

for i in range(x):
    # Read each line of input
    [a1, a2, a3] = input().split() # Be careful, a1, a2 and a3 are strings
    temp_tuple = (int(a1), int(a2), int(a3)) # Convert a1, a2 and a3 to a tuple of ints
    my_list.append(temp_tuple) # Add the tuple to your list
```

For printing output
```python
print(a, b, c)
```

## C++ Guide

You will require the following libraries

```c++
#include <iostream> // To read from input and to print output
#include <array> // To read the tuple
#include <vector> // To read the lines of input
```

To read the first line of input

```c++
int x;
std::cin >> x;
```

To read the subsequent 2 lines of input
```c++
std::vector<int> v(x); // Initialise vector with size x
for (int i = 0; i < x; ++i)
{
    std::cin >> a1 >> a2 >> a3;
    v.at(i) = std::array<int, 3>{ a1, a2, a3 }; // Assign element at i index of vector to array of inputs
}
```

To print to output

```c++
std::cout << a << b << c;
```