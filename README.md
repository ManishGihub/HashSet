
# ☕ Java HashSet

![Java](https://img.shields.io/badge/Language-Java-orange?style=for-the-badge&logo=openjdk)
![Collections](https://img.shields.io/badge/Concept-Collections-blue?style=for-the-badge)
![Level](https://img.shields.io/badge/Level-Beginner-success?style=for-the-badge)

---

## 📖 About

This repository demonstrates the basic operations of the **HashSet** class in Java's Collections Framework.

It is designed to help beginners understand how HashSet works, handles duplicate elements, and performs different operations on a collection of unique elements.

## 🧠 What is HashSet?

`HashSet` is a class in Java that implements the `Set` interface.

It uses a hash table internally to store elements and does not allow duplicate values.

### ✨ Key Features

- **Unique Elements:** Does not allow duplicate values.
- **No Insertion Order:** Does not guarantee the order of elements.
- **Null Support:** Allows one `null` element.
- **Fast Operations:** Provides average constant-time performance for basic operations.
- **Dynamic Size:** Automatically grows as elements are added.

---

## 🛠️ Operations Demonstrated

| Method | Description |
| :--- | :--- |
| `add()` | Adds an element to the HashSet. |
| `contains()` | Checks whether an element exists. |
| `remove()` | Removes an element from the HashSet. |
| `iterator()` | Creates an iterator to traverse elements. |
| `hasNext()` | Checks whether more elements are available. |
| `next()` | Returns the next element. |

---

## 💻 Code Implementation

```java
import java.util.*;

public class Hashset {
    public static void main(String[] args) {

        // Creating a HashSet
        HashSet<Integer> set = new HashSet<>();

        // Adding elements
        set.add(1);
        set.add(2);
        set.add(3);
        set.add(4);
        set.add(1);

        // Printing HashSet
        System.out.println(set);

        // Checking elements
        System.out.println(set.contains(3));
        System.out.println(set.contains(5));

        // Removing an element
        set.remove(4);

        System.out.println(set);

        // Iterating through HashSet
        Iterator<Integer> it = set.iterator();

        while (it.hasNext()) {
            System.out.println(it.next());
        }
    }
}
```

---

## 📤 Sample Output

```text
[1, 2, 3, 4]
true
false
[1, 2, 3]
1
2
3
```

> **Note:** HashSet does not maintain insertion order. The output order may vary.

---

## 🔍 How Does It Work?

1. **Creation:** Creates a HashSet of Integer type.
2. **Insertion:** Adds elements using the `add()` method.
3. **Duplicate Handling:** Ignores the duplicate value `1`.
4. **Searching:** Uses `contains()` to check whether an element exists.
5. **Deletion:** Removes an element using `remove()`.
6. **Traversal:** Uses an Iterator to access elements one by one.

---

## 🎯 Learning Objectives

By exploring this project, you will learn:

- Fundamentals of Java Collections Framework.
- Understanding the `Set` interface.
- Working with the `HashSet` class.
- Handling duplicate elements.
- Adding, searching, and removing elements.
- Iterating through collections using an Iterator.

---

## 🚀 Getting Started

### Prerequisites

- Java Development Kit (JDK).
- Basic knowledge of Java programming.
- Any Java-supported IDE or code editor.

### Installation and Execution

**1. Clone the repository**

```bash
git clone https://github.com/YOUR-USERNAME/Hashset.git
```

**2. Navigate to the project directory**

```bash
cd Hashset
```

**3. Compile the Java file**

```bash
javac Hashset.java
```

**4. Run the program**

```bash
java Hashset
```

---

## 📚 Related Java Collections

| Collection | Description |
| :--- | :--- |
| `HashSet` | Stores unique elements without guaranteeing order. |
| `LinkedHashSet` | Maintains insertion order. |
| `TreeSet` | Stores unique elements in sorted order. |

---

## 🌱 Future Enhancements

- HashSet with String values.
- HashSet with custom objects.
- Union, intersection, and difference operations.
- Comparison between HashSet, LinkedHashSet, and TreeSet.
- Exploring additional methods like `clear()` and `isEmpty()`.

---

## 🤝 Contributions

Suggestions and improvements are always welcome!

Feel free to fork this repository, explore the concepts, and submit a pull request.

## ⭐ Support

If this repository helps you understand Java HashSet, consider giving it a ⭐ on GitHub!

---

**Happy Coding! 💻☕**
