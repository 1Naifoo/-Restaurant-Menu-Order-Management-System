# Restaurant Menu & Order Management System 🍔📋

[cite_start]A high-performance command-line application developed in **C++** for the *Data Structures and Algorithms* (CSEB3213) course at **Universiti Tenaga Nasional (UNITEN)**[cite: 1973, 1975, 1977]. [cite_start]This system optimizes restaurant floor workflows by providing administrative staff with programmatically structured modules to manage dynamic menus and process incoming customer orders[cite: 1991, 1992].

> 📁 **Repository Notice:** The full target codebase implementation (**`main.cpp`**) and the official technical systems report are fully available and hosted directly within this repository's root files section.

---

## 🌟 Data Structures & Algorithmic Foundations

To ensure minimal runtime overhead and reliable data manipulation, the system is engineered entirely around fundamental **Standard Template Library (STL)** structures and standard computer science algorithms:

* [cite_start]**Dynamic Storage Arrays (`std::vector`):** Utilized to maintain contiguous, easily resizable database records for live menu item tracking and individual customer order components[cite: 1999, 2007, 2017].
* [cite_start]**Sequential FIFO Data Pipelines (`std::queue`):** Enforces a strict *First-In, First-Out* execution matrix to log, monitor, and clear customer transactions sequentially as they hit the kitchen queue[cite: 1999, 2017, 2020].
* [cite_start]**Logarithmic Search Traversal ($O(\log n)$):** Integrates a pure **Binary Search** routine to quickly target specific item keys within the menu vector during deletion updates[cite: 2000, 2011].
* [cite_start]**Data Sorting Engine:** Employs a **Selection Sort** algorithm to programmatically arrange active menu vectors by either identification tags or base pricing matrices[cite: 2000, 2003].

---

## 🛠️ System Modules

[cite_start]The application architecture is cleanly decoupled into eight independent core modules[cite: 2001]:

### Menu Management
1.  [cite_start]**Display Menu:** Accesses the active menu vector to output descriptive grids (ID, name, price)[cite: 2003, 2004]. [cite_start]Supports sorting toggles by Unique ID or Price point[cite: 2003].
2.  [cite_start]**Add Menu Item:** Appends fresh elements to the menu array after verifying that the structural properties (Unique ID, name, price string) are valid[cite: 2005, 2006].
3.  [cite_start]**Delete Menu Item:** Purges targeted nodes from the menu vector utilizing the high-efficiency binary search engine to locate records by ID[cite: 2010, 2011].
4.  [cite_start]**Edit Menu Item:** Mutates pre-existing data pointers in place to quickly modify active item names or retail pricing details[cite: 2012, 2013].

### Transaction Processing
5.  [cite_start]**Create Order:** Generates a unique transaction ticket container (vector of items), automatically aggregates item costs, and pushes the completed block into the kitchen processing line[cite: 2015, 2016, 2017].
6.  [cite_start]**View Orders:** Sequentially scans active items pending completion in the processing queue, printing distinct transaction lists alongside full invoice totals[cite: 2018, 2019].
7.  [cite_start]**Delete Order:** Pops the frontmost completed transaction block out of the queue, systematically clearing the bottleneck while maintaining exact queue guidelines[cite: 2021, 2022].
8.  [cite_start]**Edit Order:** Intercepts the primary order object currently occupying the front index of the queue, allowing staff to update its structural contents on the fly[cite: 2023, 2024].

---

## 💻 Technical Specifications Matrix

| Metric / Parameter | Implementation Detail | Operational Purpose |
| :--- | :--- | :--- |
| **Primary Language** | C++ (Standard ISO/IEC C++11 or higher) | Low-level memory management and raw execution speed. |
| **Menu Collection Type** | `std::vector<MenuItem>` | Constant time $O(1)$ random access memory indexing loops. |
| **Order Pipeline Type** | `std::queue<Order>` | Maintaining temporal chronological sequence for customer rows. |
| **Search Complexity** | $O(\log n)$ (Binary Search) | Fast element pointer location inside long data arrays. |
| **Data Integrity Rule** | Unique Entity Constraints | Validates unique menu IDs to protect data integrity across lists. |

---

## 🚀 Step-by-Step Compilation & Execution Guide

To build and run this command-line tool on your local workstation, execute the following steps:

### Prerequisites
Ensure you have an active C++ compiler installed on your system path (e.g., **GCC/G++** or **Clang**).

### Compilation Pipeline
Open your terminal inside the project directory and run the standard compilation command:
```bash
g++ -std=c++11 main.cpp -o RestaurantSystem
