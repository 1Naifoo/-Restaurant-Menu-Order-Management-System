# Restaurant Menu and Order Management System 🍔📋

[cite_start]A command-line software solution developed in **C++** for a Data Structures project (CSEB3213) at **Universiti Tenaga Nasional (UNITEN)**[cite: 1973, 1975, 1991]. [cite_start]This system optimizes day-to-day restaurant workflows by providing administrative staff with efficient, programmatically structured tools to manage dynamic menus and process sequential customer orders[cite: 1991, 1992].

> [cite_start]📁 **Note:** The complete codebase implementation (**`main.cpp`**) and the comprehensive project documentation (covering system design charts, responsibilities breakdown, and the functional logic flowchart) are available directly within this repository's files section[cite: 2030, 2048].

---

## 🌟 Architecture & Core Modules

The application utilizes core algorithmic paradigms and memory-efficient Standard Template Library (STL) data structures to deliver low-overhead data manipulation:

* [cite_start]**Dynamic Storage:** Built entirely around the **STL Vector** wrapper class to maintain contiguous, resizable elements for live menu item sets and internal order contents[cite: 1999, 2007, 2017].
* [cite_start]**FIFO Order Processing:** Implements an **STL Queue** structure to log, monitor, and process transactions sequentially in a precise First-In, First-Out manner[cite: 1999, 2017, 2020].
* [cite_start]**Optimized Data Search:** Integrates the **Binary Search** algorithm to handle lookup targets with low worst-case logarithmic runtime complexity, $O(\log n)$[cite: 2000].
* [cite_start]**Data Sorting Matrix:** Implements **Selection Sort** routines to arrange active vector structural properties systematically[cite: 2000].

---

## 🛠️ System Modules

[cite_start]The system is compartmentalized into eight distinct functional operational modules[cite: 2001]:

1.  [cite_start]**Display Menu:** Pulls from the central vector to display item IDs, names, and pricing logs[cite: 2003, 2004]. [cite_start]Supports toggling selection lists sorted cleanly either by unique ID numbers or raw base pricing values[cite: 2003].
2.  [cite_start]**Add Menu Item:** Appends incoming menu items dynamically into the target vector after validating unique user-defined ID tags, item names, and custom base pricing metrics[cite: 2006, 2007].
3.  [cite_start]**Delete Menu Item:** Queries the menu collection utilizing a high-efficiency binary search filter to pinpoint and purge old item entries via their unique identification code[cite: 2011].
4.  [cite_start]**Edit Menu Item:** Rewrites parameters directly inside the vector array to dynamically update active pricing or naming conventions for pre-existing items[cite: 2013, 2014].
5.  [cite_start]**Create Order:** Generates distinct sub-vectors containing targeted customer selections, computes item aggregation costs, and pushes the final order payload straight to the transaction queue[cite: 2016, 2017].
6.  [cite_start]**View Orders:** Sequentially reads active items pending processing inside the queue, explicitly itemizing all internal items along with total accumulated invoice receipts[cite: 2019, 2020].
7.  [cite_start]**Delete Order:** Removes the frontmost completed order block from the transaction queue, preserving standard sequential line rules[cite: 2021, 2022].
8.  [cite_start]**Edit Order:** Intercepts the primary order record at the head of the FIFO queue, allowing operators to instantly swap parameters out for a fresh set of selected items[cite: 2024].

---

## ⚙️ Execution Architecture Flow
