# CPU Scheduler Project

## Project's Title
**CPU Scheduler Project**

## Project Description
This project implements six CPU scheduling algorithms using the Qt Creator framework in C++. The scheduling algorithms implemented are:

1. **FCFS (First Come First Served)**
2. **PSJF (Preemptive Shortest Job First)**
3. **NPSJF (Non-Preemptive Shortest Job First)**
4. **PP (Preemptive Priority)**
5. **NPP (Non-Preemptive Priority)**
6. **RR (Round Robin)**

The project provides a graphical user interface (GUI) that allows users to input the number of processes, select a scheduling algorithm, and enter additional parameters such as time quantum for Round Robin scheduling.

## How to Run the Project

### Dependencies
To run this project, you need the following dependencies:

- Qt Creator (version 5.15 or higher recommended)
- C++17 compatible compiler

### Steps to Run
1. **Install Qt Creator**: Download and install Qt Creator from [Qt's official website](https://www.qt.io/download).
2. **Clone the Repository**: Clone the project repository to your local machine. ( git clone https://github.com/yourusername/cpu-scheduler.git )
3. **Open the Project in Qt Creator**:
- Launch Qt Creator.
- Open the `Cpu_scheduler.pro` file in Qt Creator.
4. **Build the Project**:
- Configure the project kit as needed.
- Click the "Build" button to compile the project.
5. **Run the Project**:
- Click the "Run" button to start the application.

## Internal Working of the Project

### Theory of CPU Scheduling Algorithms
1. **FCFS (First Come First Served)**: Processes are executed in the order they arrive in the ready queue.
2. **PSJF (Preemptive Shortest Job First)**: The process with the shortest remaining time is executed next, preempting the current process if necessary.
3. **NPSJF (Non-Preemptive Shortest Job First)**: The process with the shortest burst time is executed next without preemption.
4. **PP (Preemptive Priority)**: Processes are selected based on priority. If a new process with a higher priority arrives, it preempts the current process.
5. **NPP (Non-Preemptive Priority)**: Processes are selected based on priority, but once a process starts, it runs to completion.
6. **RR (Round Robin)**: Each process is assigned a fixed time slice (quantum). Processes are executed in a cyclic order, and if a process does not finish within its quantum, it is moved to the back of the queue.

### GUI Implementation
The project uses Qt Widgets for the GUI. The `MainWindow` class handles the main interface, allowing users to input the number of processes, select a scheduling algorithm, and input the quantum for Round Robin scheduling. The interface includes input validation to ensure correct data entry.

Key UI Elements:
- **ComboBox**: For selecting the scheduling algorithm.
- **LineEdit**: For inputting the number of processes and time quantum.
- **PushButtons**: For submitting input and canceling the operation.
- **TextBrowser**: For displaying instructions and information.

### Code Structure
- **main.cpp**: Initializes the application and displays the main window.
- **mainwindow.cpp**: Contains the logic for handling user input and launching the scheduling process.
- **mainwindow.ui**: Defines the layout and widgets of the main window.
- **Cpu_scheduler.pro**: The project file defining the Qt project settings.

### Learning Takeaways from the Project
- **Understanding CPU Scheduling Algorithms:** Gained in-depth knowledge of various CPU scheduling algorithms and their practical applications.
- **Qt Framework Proficiency:** Learned how to use the Qt framework to create a responsive and user-friendly GUI.
- **C++ Programming Skills:** Enhanced C++ programming skills, including object-oriented programming and GUI development.
- **Project Management:** Improved skills in managing a software project, from initial setup to final deployment.

### Resources/References
- **Qt Documentation:** Qt Documentation for understanding the framework and its components.
- **C++ Standard Library Documentation:** For using modern C++17 features.
- **Operating System Concepts by Silberschatz, Galvin, and Gagne:** For understanding the theoretical aspects of CPU scheduling algorithms.
- **Online Tutorials and Forums:** Various online resources such as Stack Overflow and Qt forums for troubleshooting and learning best practices.

