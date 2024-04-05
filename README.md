# Custom List Implementation in Python

This repository contains a custom implementation of a list data structure in Python, named `mylist`. This implementation provides similar functionality to Python's built-in list while also demonstrating some advanced features and operations.

## Features

- Creation of custom list objects (`mylist`)
- Addition (`append`) and removal (`pop`, `remove`) of elements
- Insertion (`insert`) at specific positions
- Finding (`find`) and counting (`count`) elements
- Sorting (`sort`) of elements
- Reversing (`reverse`) the list
- Copying (`copy`) the list
- Iteration over the list
- Slicing (`__getitem__`) of the list
- Concatenation (`__add__`) of two lists
- Extending (`extend`) the list with elements from another iterable

## Usage

```python
# Create a new custom list
my_list = mylist()

# Append elements to the list
my_list.append(1)
my_list.append(2)
my_list.append(3)

# Print the list
print(my_list)  # Output: [1, 2, 3]

# Remove an element from the list
my_list.pop()

# Print the modified list
print(my_list)  # Output: [1, 2]

# Insert an element at a specific position
my_list.insert(1, 5)

# Print the modified list
print(my_list)  # Output: [1, 5, 2]

# Find an element in the list
index = my_list.find(5)
print("Index of 5:", index)  # Output: Index of 5: 1

# Count occurrences of an element in the list
count = my_list.count(2)
print("Count of 2:", count)  # Output: Count of 2: 1

# Sort the list
my_list.sort()
print(my_list)  # Output: [1, 2, 5]

# Reverse the list
my_list.reverse()
print(my_list)  # Output: [5, 2, 1]

# Copy the list
new_list = my_list.copy()
print(new_list)  # Output: [5, 2, 1]

# Iterate over the list
for item in my_list:
    print(item)

# Output:
# 5
# 2
# 1

# Slice the list
sliced_list = my_list[1:]
print(sliced_list)  # Output: [2, 1]

# Concatenate two lists
concatenated_list = my_list + [6, 7]
print(concatenated_list)  # Output: [5, 2, 1, 6, 7]

# Extend the list with elements from another iterable
my_list.extend([8, 9])
print(my_list)  # Output: [5, 2, 1, 8, 9]
