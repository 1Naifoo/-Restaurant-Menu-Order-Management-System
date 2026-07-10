# Restaurant Menu and Order Management System 🍔📋

A command-line software solution developed in **C++** for a Data Structures project (CSEB3213) at **Universiti Tenaga Nasional (UNITEN)**. This system optimizes day-to-day restaurant workflows by providing administrative staff with efficient, programmatically structured tools to manage dynamic menus and process sequential customer orders.

> 📁 **Note:** The complete codebase implementation (**`main.cpp`**) and the comprehensive project documentation (covering system design charts, responsibilities breakdown, and the functional logic flowchart) are available directly within this repository's files section.

---

## 🌟 Architecture & Core Modules

The application utilizes core algorithmic paradigms and memory-efficient Standard Template Library (STL) data structures to deliver low-overhead data manipulation:

* **Dynamic Storage:** Built entirely around the **STL Vector** wrapper class to maintain contiguous, resizable elements for live menu item sets and internal order contents.
* **FIFO Order Processing:** Implements an **STL Queue** structure to log, monitor, and process transactions sequentially in a precise First-In, First-Out manner.
* **Optimized Data Search:** Integrates the **Binary Search** algorithm to handle lookup targets with low worst-case logarithmic runtime complexity, $O(\log n)$.
* **Data Sorting Matrix:** Implements **Selection Sort** routines to arrange active vector structural properties systematically.

---

## 🛠️ System Modules

The system is compartmentalized into eight distinct functional operational modules:

1.  **Display Menu:** Pulls from the central vector to display item IDs, names, and pricing logs. Supports toggling selection lists sorted cleanly either by unique ID numbers or raw base pricing values.
2.  **Add Menu Item:** Appends incoming menu items dynamically into the target vector after validating unique user-defined ID tags, item names, and custom base pricing metrics.
3.  **Delete Menu Item:** Queries the menu collection utilizing a high-efficiency binary search filter to pinpoint and purge old item entries via their unique identification code.
4.  **Edit Menu Item:** Rewrites parameters directly inside the vector array to dynamically update active pricing or naming conventions for pre-existing items.
5.  **Create Order:** Generates distinct sub-vectors containing targeted customer selections, computes item aggregation costs, and pushes the final order payload straight to the transaction queue.
6.  **View Orders:** Sequentially reads active items pending processing inside the queue, explicitly itemizing all internal items along with total accumulated invoice receipts.
7.  **Delete Order:** Removes the frontmost completed order block from the transaction queue, preserving standard sequential line rules.
8.  **Edit Order:** Intercepts the primary order record at the head of the FIFO queue, allowing operators to instantly swap parameters out for a fresh set of selected items.

---

## ⚙️ Execution Architecture Flow
