# timetable-generator

# Data Structures course : Mini project
### Exam time-table scheduling using graph coloring algorithm
    This program can be used to schedule exams for any university. For testing purposes, we have scheduled exams for all batches from First year till Third year with syllabus taken from Cummins College of Engineering for Women.
---
## Input format
* First line contains labels "Batch" , "Courses" for respective columns.
* "Batch" column contains all batches, for example First Year, Second Year etc.
* "Courses" contains all the courses that exams have to be scheduled for, for the respective batch
---
 ![alt text](data.png)
---
## Output
For a complete walkthrough our process, we've displayed the following :
* Data read from CSV file and converted it into an arraylist of arraylists.
* Vertices of resulting graph
* Resulting graph created
* Colour of each vertex after applying graph coloring
* Finally, the resulting time-table for exam
---
![alt text](output.png)
---
## Why graph coloring ?
To make an exam-timetable we have the following constraints :
* One batch cannot have the more than one subject exam scheduled in the same time-slot. 
* Number of time-slots required should be minimum.
---
* Graph-coloring proves to be a suitable approach for this, where the color represents the time slot.
* A graph is created where an edge exists between each subject for a batch so that they will have a unique color and will be assigned a unique time-slot.
* Non-adjacent vertices will be assigned repeated colors so that number of time-slots is minimum
## To use this
* Install an IDE which supports JAVA
* Open readfile.java and main.java
* Enter data in a csv file , and copy file path in main.java

## What's next?
* Add more constraints, such as capacity of lecture hall
* Use the same logic for creating a time-table for lectures, adding constraints such as teacher's time preferences, break for students etc
