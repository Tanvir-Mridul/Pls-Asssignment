
a) **Fixed Stack (C++ & JavaScript)**

Description:
This is a stack data structure with a predefined size limit. It operates using the **Last In, First Out (LIFO)** principle. The stack can hold a maximum of **N** elements. Once full, no more elements can be added until some are removed.

How It Works:

* Push: Adds an element to the top of the stack if space is available.
* **Pop:** Removes and returns the top element if the stack isn’t empty.
* If a push is attempted when the stack is full, it returns a **"Stack Overflow"** message.
* If a pop is attempted on an empty stack, it returns a **"Stack Underflow"** message.

---

### b) **Dynamic Stack (C++ & JavaScript)**

**Description:**
This stack grows as needed, allowing an unlimited number of elements (limited only by memory). It follows the LIFO model like a typical stack.

**How It Works:**

* **Push:** Adds an element to the top of the stack. The size expands automatically as elements are added.
* **Pop:** Removes and returns the top element.
* Internally, this is handled using a **vector** in C++ or a **dynamically growing array** in JavaScript.

---

### c) **Fixed Heap Array (C++ & JavaScript)**

**Description:**
This is a fixed-size array that resides in heap memory. The size is defined during initialization and cannot be changed later. It provides direct access to elements using indices.

**How It Works:**

* **Set:** Assigns a value to a specific index in the array.
* **Get:** Retrieves the value from a specific index.
* In C++, memory is allocated using `new`. In JavaScript, a fixed-length array is created.

---

### d) **Dynamic Heap Array (C++ & JavaScript)**

**Description:**
A dynamic array that automatically grows when new elements are added beyond its current capacity. It starts with an initial size and resizes itself as needed.

**How It Works:**

* **Insert:** Adds an element to the end of the array. If full, the array’s capacity is typically doubled.
* **Get:** Retrieves an element by its index.
* This resizing happens behind the scenes, offering flexibility for variable-sized data.

---

### **Summary of Operations**

* **Fixed Stack:**

  * Operates on LIFO.
  * Limited by a predefined size.
  * Push and Pop are bounded by this limit.

* **Dynamic Stack:**

  * Also LIFO-based.
  * Grows automatically as elements are added.
  * No size restriction except available memory.

* **Fixed Heap Array:**

  * Predefined size stored in heap memory.
  * Direct access through indexing.
  * Values are set or retrieved using indices.

* **Dynamic Heap Array:**

  * Resizes as needed.
  * Suitable for data of unpredictable size.
  * Insert grows the array, Get retrieves elements.

---

### **When to Use Each Type**

* **Fixed Stack:**
  Best when the maximum size is known in advance and you want to prevent resizing.

* **Dynamic Stack:**
  Ideal when the number of elements is unknown or changes frequently.

* **Fixed Heap Array:**
  Useful when you need random access to a fixed-size dataset allocated on the heap.

* **Dynamic Heap Array:**
  Suitable for applications where the number of elements varies, requiring flexible resizing.


