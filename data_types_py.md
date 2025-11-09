# 📊 Data Types and Data Management in Python

Understanding data types and how to manage them efficiently is essential for every Python developer — especially when working with data analysis, APIs, or machine learning.

---

## 🧱 1. Basic Data Types

| Type | Description | Example |
|------|-------------|---------|
| `int` | Integer numbers. | `x = 42` |
| `float` | Decimal (floating-point) numbers. | `pi = 3.14159` |
| `complex` | Complex numbers with real and imaginary parts. | `z = 2 + 3j` |
| `bool` | Boolean values (`True` / `False`). | `is_valid = True` |
| `str` | Strings (text data). | `name = "Josep"` |
| `NoneType` | Represents “nothing” or “no value”. | `result = None` |

---

## 🧩 2. Sequence Types

| Type | Description | Mutable | Example |
|------|-------------|---------|---------|
| `list` | Ordered, mutable collection. | ✅ Yes | `nums = [1, 2, 3]` |
| `tuple` | Ordered, **immutable** collection. | ❌ No | `coords = (10, 20)` |
| `range` | Sequence of numbers (usually for loops). | ❌ No | `range(0, 10)` |
| `str` | Sequence of characters. | ❌ No | `"Python"` |

### 🧮 Common Operations

```python
nums = [1, 2, 3]
nums.append(4)      # Add an element
nums.remove(2)      # Remove element 2
print(nums[0])      # Access by index
🗂️ 3. Mapping and Set Types
Type	Description	Mutable	Example
dict	Key-value pairs.	✅ Yes	user = {"name": "Josep", "age": 25}
set	Unordered unique elements.	✅ Yes	colors = {"red", "blue"}
frozenset	Immutable version of set.	❌ No	f = frozenset([1, 2, 3])

🧰 Dictionary Example
python
Copiar código
user = {"name": "Josep", "age": 25}
print(user["name"])       # Access value
user["country"] = "Spain" # Add new key
🧮 4. Type Conversion
You can convert between data types using built-in functions.

python
Copiar código
int("10")       # 10
float("3.14")   # 3.14
str(100)        # "100"
list("abc")     # ['a', 'b', 'c']
tuple([1, 2])   # (1, 2)
set([1, 1, 2])  # {1, 2}
Be careful: conversions can raise ValueError if the input is not valid (e.g., int("abc")).

🧠 5. Checking and Comparing Types
Function	Use	Example
type(obj)	Returns the type of a variable.	type(42) → <class 'int'>
isinstance(obj, type)	Checks if an object belongs to a type (or tuple of types).	isinstance(3.14, float)

Examples:

python
Copiar código
x = 10
print(type(x))                 # <class 'int'>
print(isinstance(x, (int,)))   # True
⚡ 6. Data Copying and References
Python variables reference objects — they are names bound to objects.

python
Copiar código
a = [1, 2, 3]
b = a        # b references the same list object
b.append(4)
print(a)     # [1, 2, 3, 4] — both names refer to same list
To create copies:

Shallow copy (copies the outer container, inner objects referenced):

python
Copiar código
a = [[1], [2]]
b = a.copy()
b[0].append(99)
print(a)  # [[1, 99], [2]] — inner lists still shared
Deep copy (recursively copies):

python
Copiar código
import copy
a = [[1], [2]]
b = copy.deepcopy(a)
b[0].append(99)
print(a)  # [[1], [2]] — original unchanged
When to use which depends on whether inner objects should be shared.

🧮 7. Mutable vs Immutable
Category	Data Types
Mutable	list, dict, set, bytearray
Immutable	int, float, tuple, str, frozenset, bytes

Implications:

Immutable objects can be used as dictionary keys or set elements (if hashable).

Mutable objects can change in place, which affects references and shared state.

Immutable objects are safer for concurrency and can be cached.

📦 8. Working with Collections
Python’s collections module provides advanced containers for common patterns.

Class	Description	Example
namedtuple	Tuple with named fields (lightweight, immutable).	python\nfrom collections import namedtuple\nPoint = namedtuple("Point", "x y")\np = Point(1, 2)\nprint(p.x)\n
deque	Double-ended queue with fast appends/pops from both ends.	python\nfrom collections import deque\nq = deque([1,2,3])\nq.appendleft(0)\nq.pop()\n
Counter	Counts occurrences of elements in an iterable.	python\nfrom collections import Counter\nCounter('banana') # Counter({'a':3, 'n':2, 'b':1})\n
defaultdict	Dict that provides default values for missing keys.	python\nfrom collections import defaultdict\nd = defaultdict(int)\nd['x'] += 1\n

Use these when you need performance or convenience patterns beyond built-in list/dict/set.

🧰 9. Working with DataFrames and External Data (Intro)
For structured tabular data, pandas is the standard library in Python ecosystem. numpy provides efficient numeric arrays.

Basic pandas example:

python
Copiar código
import pandas as pd

df = pd.DataFrame({
    "name": ["Ana", "Josep", "Leo"],
    "age": [22, 25, 30]
})
print(df.head())
Key tips:

Use df.info() and df.describe() to inspect types and statistics.

Convert types explicitly: df['age'] = df['age'].astype(int)

Handle missing data: df.dropna() or df.fillna(value)

📘 10. Summary
Understand how Python stores and handles mutable vs immutable types.

Use dict, set, and comprehensions for efficient data manipulation.

Be careful with references; use shallow or deep copy appropriately.

collections offers powerful alternatives for common data patterns.

For real-world data work, learn pandas and numpy (inspect types, convert, handle missing values).

Author: Josep
Purpose: Quick and complete reference for Python data types and data management.
