#  Banker's Algorithm

An animation of the **Banker’s Algorithm**, a classic **deadlock avoidance** algorithm used in operating systems.  
It helps determine whether a system is in a **safe state** by simulating resource allocation for multiple processes.

---

##  Overview

The **Banker’s Algorithm** is used to ensure that resource allocation in a system does not lead to a **deadlock**.  
It checks if granting a resource request will leave the system in a safe state where all processes can complete.

This project demonstrates:
- Safe state detection  
- Resource allocation and deallocation  
- Deadlock prevention logic  

---

##  Features

- Accepts user input for:
  - Number of processes and resource types  
  - Allocation matrix  
  - Maximum demand matrix  
  - Available resources  

- Computes:
  - **Need Matrix**
  - **Safe Sequence** (if it exists)

- Displays detailed step-by-step output showing:
  - Work vector updates  
  - Finish status of processes  
  - Safe/Unsafe system status  

---

##  Example Input

Enter the number of processes: 5
Enter the number of resources: 3
Enter the Allocation Matrix:
0 1 0
2 0 0
3 0 2
2 1 1
0 0 2
Enter the Max Matrix:
7 5 3
3 2 2
9 0 2
2 2 2
4 3 3
Enter Available Resources:
3 3 2

---

##  Example Output

Need Matrix:
7 4 3
1 2 2
6 0 0
0 1 1
4 3 1
System is in a SAFE STATE.
Safe Sequence: <P1, P3, P4, P0, P2>

---

##  Concepts Used

- **Deadlock Avoidance**
- **Resource Allocation Graph**
- **Safe Sequence Detection**
- **Matrix Representation in C/C++**

---

##  How to Run

1. Clone or download this repository:
   ```bash
   git clone https://github.com/yourusername/bankers-algorithm.git
Navigate to the project folder:
cd bankers-algorithm
Compile the program:
gcc bankers_algorithm.c -o bankers
or for C++:
g++ bankers_algorithm.cpp -o bankers
Run the program:
./bankers
📄 File Structure
📂 Bankers-Algorithm
 ┣ 📜 bankers_algorithm.cpp
 ┣ 📜 README.md
 ┗ 📜 sample_input.txt
💡 Future Improvements
Add GUI to visualize resource allocation.
Integrate request handling dynamically during runtime.
Implement a simulator web app using React or Node.js.
👩‍💻 Author
Diya Shrestha
🎓 BTech in Computer Science and Engineering
💬 “Avoiding deadlocks, one process at a time.”
🪶 License
This project is open-source under the MIT License.
MIT License © 2025 Diya Shrestha
