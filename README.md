# University Inventory Management System
 
> **Student:** Krishal Acharya  
> **Institution:** National Academy of Professional Studies (NAPS)

---

## Project Overview

Welcome to my **University Inventory Management System**! 

This is a console-based Java application designed to help university staff manage thousands of assets—from computers to laboratory equipment. In the real world, tracking who has what equipment and when it's due for maintenance is a nightmare. This system solves that by simulating a central hub where you can:

* **Track Assets:** Manage Equipment, Furniture, and Lab gear.
* **Assign Items:** Check equipment out to staff members (with strict limits!).
* **Monitor Status:** specific tracking for warranties, maintenance schedules, and overdue fees.

I built this project to demonstrate my understanding of core Java concepts, moving from basic loops all the way to complex Object-Oriented Programming principles.

---

## Key Features

* **Asset Management:** Add different types of inventory (Standard Equipment, Furniture, Lab Equipment) using a polymorphic design.
* **Staff & Assignments:** Register staff and assign them up to **5 items**. The system automatically blocks assignments if they exceed this limit.
* **Smart Search:** Find items by name, category, or warranty status using method overloading.
* **Automated Reports:** Generate instant reports for:
    * Current inventory status.
    * Items with expired warranties (so we know what to replace!).
    * Maintenance schedules.
* **Robust Error Handling:** The system uses custom exceptions (like `AssignmentLimitExceededException`) to handle errors gracefully without crashing.

---

## Project Structure

I organized the code into packages to keep the logic clean and maintainable:

```text
UniversityInventorySystem/
 ├── src/
 │   ├── models/           # The blueprints (Equipment, StaffMember, etc.)
 │   ├── managers/         # The logic (InventoryManager, InventoryReports)
 │   ├── exceptions/       # Custom error handling classes
 │   └── UniversityInventorySystem.java  # The main application entry point
 ├── README.md
 └── .gitignore
