# Restaurant Menu & Order Management System 🍔📋

A performance-focused command-line application developed in **C++** for the *Data Structures and Algorithms* (CSEB3213) course at **Universiti Tenaga Nasional (UNITEN)**. This system optimizes day-to-day restaurant workflows by providing administrative operators with programmatically structured modules to manage dynamic menus and process incoming sequential customer orders.

> 📁 **Repository Notice:** The complete source codebase implementation (**`main.cpp`**) and the official technical systems report are fully available and hosted directly within this repository's root files section.

---

## 🌟 Data Structures & Algorithmic Foundations

To ensure minimal runtime overhead and reliable data manipulation under load, the application is engineered entirely around fundamental **Standard Template Library (STL)** structures and classical computer science algorithms:

* **Dynamic Storage Arrays (`std::vector`):** Utilized to maintain contiguous, easily resizable data elements for live menu item sets and individual customer order components.
* **Sequential FIFO Data Pipelines (`std::queue`):** Enforces a strict *First-In, First-Out* execution matrix to log, monitor, and clear transactions sequentially as they enter the kitchen processing line.
* **Logarithmic Search Traversal ($O(\log n)$):** Integrates a pure **Binary Search** routine to target specific item keys within the menu vector rapidly during deletion or verification updates.
* **Data Sorting Engine:** Employs a **Selection Sort** algorithm to programmatically arrange active menu vectors by either unique identification tags or base pricing matrices.

---

## 🛠️ System Modules

The application architecture is decoupled into eight independent core operational modules:

### Menu Management
1. **Display Menu:** Accesses the active menu vector to output descriptive grids containing item IDs, names, and pricing logs. Supports sorting toggles by Unique ID or raw price points.
2. **Add Menu Item:** Appends fresh elements to the menu array dynamically after validating unique user-defined ID tags, item names, and custom base pricing metrics.
3. **Delete Menu Item:** Purges targeted elements from the menu vector utilizing the high-efficiency binary search engine to locate records smoothly by their ID.
4. **Edit Menu Item:** Mutates pre-existing data pointers in place to modify active item names or retail pricing details instantly without restructuring the collection.

### Transaction Processing
5. **Create Order:** Generates a unique transaction ticket container (vector of selected menu items), automatically aggregates items to calculate final invoice costs, and pushes the completed payload into the kitchen queue.
6. **View Orders:** Sequentially scans active items pending fulfillment in the processing queue, explicitly itemizing all internal entries alongside total accumulated invoice receipts.
7. **Delete Order:** Pops the frontmost completed transaction block out of the queue, systematically clearing the bottleneck while maintaining exact FIFO queue guidelines.
8. **Edit Order:** Intercepts the primary order object currently occupying the front index of the queue, allowing operators to update its structural contents on the fly before final processing.

---

## 💻 Technical Specifications Matrix

| Metric / Parameter | Implementation Detail | Operational Purpose |
| :--- | :--- | :--- |
| **Primary Language** | C++ (Standard ISO/IEC C++11 or higher) | Low-level memory efficiency and clean execution speed. |
| **Menu Collection Type** | `std::vector<MenuItem>` | Constant time $O(1)$ random access memory indexing loops. |
| **Order Pipeline Type** | `std::queue<Order>` | Maintaining strict temporal chronological sequence for incoming queues. |
| **Search Complexity** | $O(\log n)$ (Binary Search) | Rapid element pointer location inside large data arrays. |
| **Data Integrity Rule** | Unique Entity Constraints | Validates unique menu IDs to protect data integrity across lists. |

---

## 🚀 Step-by-Step Compilation & Execution Guide

To build and run this command-line tool on your local workstation, execute the following steps:

### Prerequisites
Ensure you have an active C++ compiler installed on your system path (such as **GCC/G++** or **Clang**).

### Compilation Pipeline
Open your terminal inside the project directory and execute the standard compilation command:
```bash
g++ -std=c++11 main.cpp -o RestaurantSystem
