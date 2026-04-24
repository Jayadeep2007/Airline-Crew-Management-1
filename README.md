# ✈️ Airline Crew Management System

## 📌 Crew Assignment Graph CRUD

A **menu-driven C program** for **Airline Crew Management** that implements full **CRUD operations** using a **Graph Data Structure** to manage crew assignments between crew members.

---

## 👥 Team Members

- **Thirumala Reddy** – Lead Developer  
- **Jaydeep Ram** – Graph Implementation & Testing  

---

## 🎯 Problem Statement

Design a system to manage airline crew members and their assignment relationships efficiently using graphs.

The program supports:

- ✅ Crew Member Management (**Create, Read, Update, Delete**)
- ✅ Crew Assignments (**Directed Graph Relationships**)
- ✅ Dynamic Memory Allocation
- ✅ Proper Memory Cleanup
- ✅ Robust Input Validation
- ✅ Error Handling

---

## 🏗️ Data Structures Used

### 1️⃣ Crew Node (Primary Linked List)


typedef struct Crew {
    int id;                 // Unique crew ID
    char name[50];          // Crew member name
    struct Crew* next;      // Next crew in list
    struct AdjList* adj;    // Adjacency list for assignments
} Crew;
2️⃣ Adjacency List Node (Graph Edges)  :


 typedef struct AdjList {
    struct Crew* dest;      // Destination crew member
    struct AdjList* next;   // Next assignment
} AdjList;

⚙️ Features
1.Add New Crew Members
2.Delete Existing Crew Members
3.Update Crew Details
4.Search Crew by ID
5.Display Crew Assignment Graph
6.Add Directed Assignments Between Crew Members
7.Menu Driven Interface

📊 Time Complexity  :

| Operation      | Time Complexity | Space Complexity |
| -------------- | --------------- | ---------------- |
| Add Crew       | O(1)            | O(1)             |
| Delete Crew    | O(n)            | O(1)             |
| Update Crew    | O(n)            | O(1)             |
| Search Crew    | O(n)            | O(1)             |
| Display Graph  | O(V + E)        | O(1)             |
| Add Assignment | O(n)            | O(1)             |


🖥️ Compilation:

• GCC Compiler (Linux / Mac / Windows with MinGW)
• Standard C Library
 

📋 Menu Interface  :

====================================
 ✈ AIRLINE CREW MANAGEMENT SYSTEM
====================================
1. Add Crew (Create)
    <img width="362" height="257" alt="Screenshot 2026-04-24 at 11 05 21 PM" src="https://github.com/user-attachments/assets/98252187-0e5f-4075-9fd0-1f23334bbec0" />

2. Delete Crew
    <img width="362" height="244" alt="Screenshot 2026-04-24 at 11 09 16 PM" src="https://github.com/user-attachments/assets/356eea03-d69a-433c-a1cb-31529eec95d7" />

3. Update Crew
    <img width="334" height="258" alt="Screenshot 2026-04-24 at 11 11 22 PM" src="https://github.com/user-attachments/assets/0789ff4f-883f-45e3-b207-6660146fcc56" />

4. Search Crew
    <img width="344" height="264" alt="Screenshot 2026-04-24 at 11 12 44 PM" src="https://github.com/user-attachments/assets/d39e0333-36bb-4ca9-8980-cc7e1e2dfa78" />

5. Display Graph
    <img width="350" height="250" alt="Screenshot 2026-04-24 at 11 15 42 PM" src="https://github.com/user-attachments/assets/5cc510fe-9360-4491-a261-9ab579926238" />

6. Add Assignment
    <img width="352" height="260" alt="Screenshot 2026-04-24 at 11 18 53 PM" src="https://github.com/user-attachments/assets/b70a3919-c377-494c-817d-22d1236803a0" />

7. Exit
    <img width="349" height="195" alt="Screenshot 2026-04-24 at 11 20 06 PM" src="https://github.com/user-attachments/assets/f086d0a0-1586-4e0b-b58b-2ae36fa1854c" />

====================================

📌 Sample Output :  

Enter Choice: 1

Enter Crew ID: 101
Enter Crew Name: Captain Smith
✅ Crew Added Successfully!

Enter Choice: 1

Enter Crew ID: 102
Enter Crew Name: Co-Pilot Jones
✅ Crew Added Successfully!

Enter Choice: 6

Enter Source Crew ID: 101
Enter Destination Crew ID: 102
✅ Assignment Added!

Enter Choice: 5

--- Crew Assignment Graph ---
Crew 102 (Co-Pilot Jones) ➝
Crew 101 (Captain Smith) ➝ 102

Enter Choice: 4

Enter Crew ID to Search: 101
🔍 Found → ID: 101 | Name: Captain Smith

Demo Video Link  :



  

