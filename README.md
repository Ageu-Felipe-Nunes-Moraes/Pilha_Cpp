# Stack - C++ Implementation

This project consists of a simple implementation of a stack in C++. A stack is a data structure that follows the "Last In, First Out" (LIFO) principle, where the last element added is the first to be removed.

## Features

- **Push:** Adds an item to the top of the stack.
- **Pop:** Removes the item from the top of the stack, if any.
- **Top:** Returns the item from the top of the stack without removing it.
- **Empty:** Checks if the stack is empty.

## How to Use

1. Instantiate an object of the `Stack` class.
2. Add elements to the stack using the `push(item)` method.
3. Remove elements from the stack using the `pop()` method.
4. Retrieve the top element without removing it using the `top()` method.
5. Check if the stack is empty using the `empty()` method.

## Example Usage

```Cpp
int main(){
    // Declare an object of the class
    Stack stack;

    // Fill the list with 100 numbers
    for (int i = 0; i < 101; i++) {
        stack.push(i);
        stack.printList();
        stack.sleepForOneSecond();
    }
    cout << endl;

    stack.printList();
    cout << "Please wait..." << endl;
    stack.sleepForOneSecond();

    // Emptying the entire list
    while (not stack.empty()){
        int last_item_list = stack.top();
        stack.pop();
        cout << "Item successfully removed from the list: " << last_item_list << endl;
        stack.printList();
        stack.sleepForOneSecond();
    }

    return 0;
}
```
This example demonstrates how to fill a stack with numbers from 0 to 100, print the stack, wait for a few seconds, and then remove each element from the stack while printing the resulting stack.

## Author

This code was developed by Ageu Felipe Nunes Moraes (myself) as part of a personal project dedicated to strengthening and maturing coding skills. For any questions or suggestions, please contact me at [ageumoraes67@gmail.com](mailto:ageumoraes67@gmail.com).

## Disclaimer

This is a software project developed by an individual and has no affiliation with any other entity.
