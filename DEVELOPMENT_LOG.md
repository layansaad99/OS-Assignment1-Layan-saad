# Development Log

### Entry 1 - [March 27, 2026, 10:00 AM]
**What I did**: Set up GitHub and forked the repository

**Details**: 
Created GitHub account with my university email. Forked the starter repository and renamed it. Installed JDK and set up VS Code.

**Challenges**: Java wasn't working at first

**Solution**: Downloaded JDK 17 and added it to PATH

**Time spent**: 30 minutes

---

### Entry 2 - [March 28, 2026, 2:00 PM]
**What I did**: Changed student ID and studied the code

**Details**: 
Set my student ID (445052146) in SchedulerSimulation.java. Ran the program to see how it works. Read through both classes to understand the logic.

**Challenges**: Understanding the relationship between Thread and Process

**Solution**: Added comments and traced the flow step by step

**Time spent**: 1 hour

---

### Entry 3 - [March 28, 2026, 3:00 PM]
**What I did**: Added Process Priority feature

**Details**: 
Added priority variable to Process class. Updated constructor and made random priorities between 1-5. Changed addProcessToQueue() to show priority.

**Challenges**: Making sure random generation worked with existing seed

**Solution**: Used random.nextInt(5) + 1 with the existing Random object

**Time spent**: 45 minutes

---

### Entry 4 - [March 29, 2026, 2:00 PM]
**What I did**: Added Context Switch Counter

**Details**: 
Added static int contextSwitches variable. Incremented it before starting each thread. Printed the total at the end.

**Challenges**: Deciding where to increment the counter

**Solution**: Put it right before currentThread.start()

**Time spent**: 30 minutes

---

### Entry 5 - [March 29, 2026, 4:00 PM]
**What I did**: Added Waiting Time Tracking

**Details**: 
Added totalWaitingTime variable and addWaitingTime() method. Tracked quantum start time and calculated waiting time for processes in queue. Fixed duplicate entries in summary.

**Challenges**: Processes were showing up multiple times in the summary

**Solution**: Used HashMap to store each process only once before printing

**Time spent**: 1 hour

---

### Entry 6 - [March 30, 2026, 6:00 PM]
**What I did**: Recorded video and finished documentation

**Details**: 
Recorded 2-minute video showing code and execution. Uploaded to Google Drive. Completed all documentation files.

**Challenges**: Keeping video under 3 minutes

**Solution**: Practiced explanation twice before recording

**Time spent**: 1 hour

---

## Summary

**Total time spent**: About 5-6 hours

**Most challenging part**: Waiting time tracking and fixing duplicate entries

**Most interesting learning**: Seeing how Round-Robin actually works with real output

<<<<<<< HEAD
**What I would do differently**: Make more commits and test more frequently
=======
**What I would do differently**: Make more commits and test more frequently
>>>>>>> c60934b83d7fbd907c1344dc8601c24bb4fdfa3f
