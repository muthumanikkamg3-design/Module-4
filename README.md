# Classes and Objects in Python: Calculate the Area of a Circle

## 🎯 Aim
To write a Python program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `cse` and a method `mech` to perform the calculation.

## 🧠 Algorithm
1. **Get user input**: Take the radius of the circle as input from the user.
2. **Define the class**: Create a class named `cse`.
3. **Define the method**: Inside the class, define the method `mech` to calculate the area of the circle using the formula:  
   Area = pi *r^2 
4. **Execute the program**: Create an object of the class and call the method with the radius value.

## 🧾 Program
~~~
import math

class cse:
    def mech(self, r):
        area = math.pi * r * r
        print("Area of Circle =", area)

radius = float(input("Enter the radius: "))

obj = cse()
obj.mech(radius)
~~~

## Output
<img width="1361" height="145" alt="image" src="https://github.com/user-attachments/assets/a3f43692-c973-41d5-843d-e127307d61da" />


## Result
Thus the program has been successfully executed


## Dictionary Operations in Python: Merging Two Dictionaries

## 🎯 Aim
To write a Python program that merges **two dictionaries** and combines their key-value pairs.

## 🧠 Algorithm
1. Define two dictionaries `dict1` and `dict2` with some key-value pairs.
2. Define a function `merge()` that merges the two dictionaries using the `**` unpacking operator.
   - The merged result will combine keys from both dictionaries. If a key exists in both, the value from `dict2` will overwrite that from `dict1`.
3. Call the `merge()` function and print the merged dictionary.

## 🧾 Program

~~~
dict1 = {'Ten': 10, 'Twenty': 20, 'Thirty': 30}
dict2 = {'Thirty': 30, 'Fourty': 40, 'Fifty': 50}

def merge(dict1, dict2):
    res = {**dict1, **dict2}
    return res

dict3 = merge(dict1, dict2)
print(dict3)
~~~

## Output
<img width="1446" height="137" alt="image" src="https://github.com/user-attachments/assets/b7e0eb08-fd18-4ef2-bdba-1d4edf3912be" />

## Result
thus,the program has been executed successfully.



# 🔤 Dictionary-Python Program to Sort a Dictionary by Keys and Values

This Python program demonstrates how to sort a dictionary:
- Alphabetically by keys
- Alphabetically by values

---

## 🎯 Aim

To write a Python program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order

---

## 🧠 Algorithm

1. **Start the program.**
2. **Define** a dictionary with key-value pairs.
3. **Sort by Keys**:
   - Use `sorted(dictionary.items())`
   - Convert the result to a dictionary using `dict()`
4. **Sort by Values**:
   - Use `sorted(dictionary.items(), key=lambda item: item[1])`
   - Convert the result to a dictionary using `dict()`
5. **Display** the original and sorted dictionaries.
6. **End the program.**

---

## 🧪Program
~~~

my_dict = {
    "banana": "yellow",
    "apple": "red",
    "grape": "green",
    "orange": "orange"
}

sorted_by_keys = dict(sorted(my_dict.items()))


sorted_by_values = dict(sorted(my_dict.items(), key=lambda item: item[1]))


print("Original Dictionary:")
print(my_dict)

print("\nDictionary Sorted by Keys:")
print(sorted_by_keys)

print("\nDictionary Sorted by Values:")
print(sorted_by_values)
~~~

## Sample Output
<img width="1387" height="382" alt="image" src="https://github.com/user-attachments/assets/d9f61b13-3a27-4639-a903-d879b4678140" />

## Result
Thus the program executed successfully.





# Exception Handling in Python: Avoiding Index Errors

## 🎯 Aim
To write a Python program that handles an **IndexError** when trying to access an element beyond the available range of a list.

## 🧠 Algorithm
1. Define a list `list1` with some integer elements.
2. Use a **try-except** block:
   - In the `try` block, attempt to access an index that is out of range (e.g., `list1[5]`).
   - In the `except` block, catch the error and print a custom message `"You're out of list range"`.
3. Print the result based on whether the index access succeeds or fails.

## 🧾 Program
~~~
try:
    L = []

    for i in range(3):
        item = input("Enter an item: ")
        L.append(item)

    print(L[4])

except IndexError:
    print("check index range")
~~~
## Output
<img width="1452" height="240" alt="image" src="https://github.com/user-attachments/assets/14b55c18-07fa-4735-8b7c-2784643fee98" />

## Result
Thus the Python program executed successfully.


# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program
~~~
def returnSum(myDict):
    final=0
    for i in myDict.values():
        final+=i
    return final
#driver functions

myDict = {'a': 100, 'b': 200, 'c': 300}
print("Sum :",returnSum(myDict))
~~~
## Output
<img width="1452" height="140" alt="image" src="https://github.com/user-attachments/assets/1bfa9bcb-1d32-43a1-843b-1a8dca62907c" />

## Result
Thus,the program has been executed successfully.
