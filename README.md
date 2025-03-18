# CPU Scheduling Visualizer

## Overview
The **CPU Scheduling Visualizer** is a web-based tool that simulates different CPU scheduling algorithms. It allows users to input processes with their respective attributes, choose a scheduling algorithm, and visualize the execution order through a Gantt chart. The tool also calculates average waiting time and turnaround time for the processes.

## Features
- **Add Processes**: Users can input process details such as Process ID, Arrival Time, Burst Time, and Priority.
- **Select Scheduling Algorithm**: Supports multiple scheduling algorithms:
  - First-Come, First-Serve (FCFS)
  - Shortest Job First (SJF) (Non-Preemptive)
  - Shortest Job First (SJF) (Preemptive)
  - Priority Scheduling
  - Round Robin (RR)
- **Gantt Chart Visualization**: Displays the execution timeline of processes.
- **Performance Metrics**: Computes and displays average waiting time and turnaround time.

## How It Works
### 1. Adding Processes
Users enter process details in the input fields and click the **Add Process** button. The process is then added to the table for tracking.

### 2. Selecting and Running a Scheduling Algorithm
Users select a scheduling algorithm from the dropdown menu and click the **Run Scheduler** button. The selected algorithm is applied to schedule the processes.

### 3. Generating the Gantt Chart
A Gantt chart is dynamically created based on the execution order of processes. It visually represents the scheduling process.

### 4. Calculating Metrics
The program computes the **Average Waiting Time** and **Average Turnaround Time** for the given processes and displays them on the webpage.

## Code Explanation
### HTML (`index.html`)
- Defines the structure of the webpage, including input fields, buttons, a table for processes, and a container for the Gantt chart.
- Provides a dropdown menu for selecting the scheduling algorithm.

### CSS (`styles.css`)
- Styles the webpage to provide a clean and user-friendly interface.
- Uses responsive design principles to ensure usability on different screen sizes.

### JavaScript (`script.js`)
- **`addProcess()`**: Collects process details from input fields and stores them in an array.
- **`updateProcessTable()`**: Updates the displayed process table whenever a new process is added.
- **`schedule()`**: Determines which scheduling algorithm to use and processes the scheduling logic accordingly.
- **`displayGanttChart()`**: Dynamically creates the Gantt chart to visualize process execution.
- **`calculateTimes()`**: Computes waiting time and turnaround time based on process execution.

## Running the Project
1. Download or clone the repository.
2. Open `index.html` in a web browser.
3. Add processes, select an algorithm, and click **Run Scheduler** to visualize the scheduling.

## Future Enhancements
- Implement additional scheduling algorithms.
- Improve UI/UX for better visualization.
- Add more performance metrics.

## Conclusion
This CPU Scheduling Visualizer is a useful tool for understanding how different CPU scheduling algorithms work. It provides an interactive and visual representation of scheduling processes, making learning more effective and engaging.

