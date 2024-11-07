
2024-11-08 01:53

Status: #Finished 

Tags: [[project management]]

# Project Planning

- PDM and CDM are used to plan, schedule, and manage tasks in a project.

1. **Precedence Diagramming Method (PDM):**
	- A graphical method to visualize relationships between the different tasks in a project
	- It uses **nodes** to represent tasks and **arrows** to depict dependencies and sequence of tasks
	- PDM includes relationships like **start-to-start, start-to-finish, finish-to-start, finish-to-finish**.
PDM is also known as **Activity On Node (AON)**.
2. **Critical Path Method (CPM)**:
	- A technique which utilizes the network of the tasks to determine the critical path. Critical path represents the **shortest time** in which the project can be completed. Any delays in this path would push the entire project beyond the deadline.
	- CPM also identifies which tasks are **crucial** to completing the project on time.
	- **==CPM gives you the shortest time but the longest path==**
CPM is also known as **Activity On Arrow (AOA)** 

## Task Relationships

There are 4 types of relationships between tasks:
1. Start-to-Start
2. Start-to-Finish
3. Finish-to-Start
4. Finish-to-Finish

## CPM

In CPM we have 2 main concepts:
1. **Critical Task**: Critical task cannot be delayed. Otherwise the project will go beyond the deadline
2. **Critical Path:** Critical path is a sequence of tasks which gives us the longest path to the end.
### **PERT CPM Method**

A single Node in CPM includes the following details:
- Activity Label
- Earliest Start 
- Earliest Finish
- Latest Start
- Latest Finish
- Float
- Duration

**Earliest Start:** For the first node the **ES** is 0. For the Next Node the **EF** of the previous node is its **ES**. In case there are 2 or more previous nodes, we'll always choose the one with the maximum **EF**.
**Earliest Finish:** **ES** + Duration
**Latest Start:** **LF** - Duration
**Latest Finish:** For the last node, **LF = EF** | For the previous nodes, **LF = LS of the next node**. Incase of 2 nodes, we choose the minimum
**Float**: **LF - EF**

There are 2 steps to this:
1. Forward Pass: In this pass we find out the **ES** and **EF** of all nodes 
2. Backward Pass: In this pass we find out the **LS** and **LF** of all nodes
 


#### References
[[Project Planning, Critical Path, Schedule Compression Techniques University Lecture.pdf]]