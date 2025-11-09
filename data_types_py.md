# 📊 Python Data Types Reference

Understanding data types and how to manage them efficiently is essential for every Python developer.

---

## 🧱 1. Basic Data Types

| Type       | Description                         | Example            |
|-----------|-------------------------------------|------------------|
| `int`     | Integer numbers.                     | `42`             |
| `float`   | Decimal (floating-point) numbers.    | `3.14159`        |
| `complex` | Complex numbers with real and imaginary parts. | `2 + 3j`      |
| `bool`    | Boolean values (`True` / `False`).  | `True`           |
| `str`     | Strings (text data).                 | `"Josep"`        |
| `NoneType`| Represents “nothing” or “no value”. | `None`           |

---

## 🧩 2. Sequence Types

| Type    | Description           | Mutable | Example       |
|--------|----------------------|---------|---------------|
| `list` | Ordered, mutable collection. | ✅ Yes  | `[1, 2, 3]` |
| `tuple`| Ordered, immutable collection. | ❌ No | `(10, 20)` |
| `range`| Sequence of numbers. | ❌ No | `range(0, 10)` |
| `str`  | Sequence of characters. | ❌ No | `"Python"` |

---

## 🗂️ 3. Mapping and Set Types

| Type        | Description             | Mutable | Example                    |
|------------|------------------------|---------|----------------------------|
| `dict`     | Key-value pairs.        | ✅ Yes  | `{"name": "Josep", "age": 25}` |
| `set`      | Unordered unique elements. | ✅ Yes | `{"red", "blue"}`         |
| `frozenset`| Immutable version of set. | ❌ No | `frozenset([1, 2, 3])`     |

---

## 🧮 4. Mutable vs Immutable Types

| Category  | Data Types |
|-----------|------------|
| Mutable   | `list`, `dict`, `set`, `bytearray` |
| Immutable | `int`, `float`, `tuple`, `str`, `frozenset`, `bytes` |

**Notes:**
- Immutable objects can be used as dictionary keys or set elements.  
- Mutable objects can change in place, which affects references and shared state.

---

## 🧠 5. Type Checking

| Function              | Description                               | Example                  |
|-----------------------|-------------------------------------------|--------------------------|
| `type(obj)`           | Returns the type of a variable.          | `type(42)` → `<class 'int'>` |
| `isinstance(obj, type)` | Checks if an object is of a specific type. | `isinstance(3.14, float)` |

---

## 📘 Summary

- Understand basic Python types: numeric, boolean, text, sequences, sets, mappings.  
- Know which types are mutable vs immutable.  
- Use `dict`, `set`, and sequences appropriately based on mutability.  
- Immutable types are safer for keys, caching, and concurrency.

**Author:** Josep  
**Purpose:** Quick reference for Python data types.
