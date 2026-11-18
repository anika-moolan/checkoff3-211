# checkoff3-211
This repository contains my work for COMP 211 Checkoff 3. My presentation is on Multilevel Feedback Queue. 

In this project, I utilized an AI tool (Claude) to develop an understanding of Multilevel Feedback Queue (MLFQ), an Operating System Scheduling Algorithm. I first defined the following basics of Operating System Scheduling:

- Operating System Scheduling happens because a computer has more processes to run than CPU cores.
- Time sharing: Switching between tasks so quickly that it looks like everything is running at the same time 


I then learned the following 5 rules of MLFQ: 
1. A new job starts at the highest priority. 
   - This promotes better response time; assumes a new job is short. 
2. Once a job uses up its time allotment at a level, its priority drops. 
   - A job that uses up its time allotment must be long and CPU-bound. 
3. If Priority(A)  > Priority(B), A runs and B doesn’t. 
   - This allows shorter jobs to go first. 
4. If Priority(A) = Priority(B), they run Round Robin. 
   - No job waits too long
5. After some time period S, every job moves up to the top queue. 
   - Ensures CPU-bound jobs still get run (starvation) and reflects current behavior of the job
  
I then used the following analogy/example to further understand this concept: 

<img width="1117" height="623" alt="Screenshot 2026-11-18 at 11 17 12 AM" src="https://github.com/user-attachments/assets/b838d857-b1db-4cec-92aa-d2c87798320f" />

My key takeaway about MLFQ was as follows: MLFQ uses a job’s past behavior to predict its future.
