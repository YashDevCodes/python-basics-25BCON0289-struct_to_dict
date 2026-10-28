# Struct-to-Dict

A simple Python project demonstrating how to convert a `namedtuple` into a dictionary using Python's built-in `_asdict()` method.

## Overview

This project creates a `Student` record using `namedtuple` and converts it into a dictionary for easier data handling and access.

## Features

- Creates a structured student record using `namedtuple`.
- Converts the record into a dictionary using `_asdict()`.
- Displays both the original student record and the converted dictionary.
- Uses Python's built-in `collections` module.

## Requirements

- Python 3.x
- No external libraries required.

## How to Run

1. Clone this repository:

   ```bash
   git clone <your-repository-url>
   ```

2. Navigate to the project directory:

   ```bash
   cd struct_to_dict
   ```

3. Run the Python file:

   ```bash
   python struct_to_dict.py
   ```

## Example Code

```python
from collections import namedtuple

Student = namedtuple("Student", ["name", "age", "course"])

student = Student("Rahul", 20, "BTech CSE")

student_dict = student._asdict()

print("Student record:", student)
print("Dictionary:", dict(student_dict))
```

## Sample Output

```text
Student record: Student(name='Rahul', age=20, course='BTech CSE')
Dictionary: {'name': 'Rahul', 'age': 20, 'course': 'BTech CSE'}
```

## Learning Objective

Understand how to use Python's `namedtuple` and `_asdict()` method to convert structured data into a dictionary.

## License

This project is open-source. Add a license file if you want to specify the terms under which others can use your code.
