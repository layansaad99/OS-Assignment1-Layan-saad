# Assignment Questions

## Question 1: Thread vs Process

**Your Answer:**

A process is a program that runs independently with its own memory space, while a thread is a smaller unit that runs inside a process and shares its memory. Threads are lighter and faster to create because they don't need new memory allocation. In this assignment, I used threads because I needed to simulate multiple processes sharing the CPU easily. In my code, I create a new Thread for each Process and manage them in a queue, which would be more complicated with separate processes.

---

## Question 2: Ready Queue Behavior

**Your Answer:**

When a process doesn't finish within its time quantum, it gets moved to the end of the ready queue to run again later. This gives other processes a chance to run and makes the scheduling fair.

**Example from my output:**
▶ P2 executing quantum [4000ms]
⏸ P2 completed quantum 4000ms │ Overall progress: [████████░░░░░░░░░░░░] 42%
Remaining time: 5316ms
↻ P2 yields CPU for context switch

➕ P2 added to ready queue │ Burst time: 9316ms | Priority: 5

text

**Explanation of example:**
P2 ran for 4000ms but still had 5316ms left. Instead of finishing, it was put back in the ready queue. This shows how Round-Robin works - processes take turns running for a fixed time slice.

---

## Question 3: Thread States

**Your Answer:**

1. **New**: When the Thread object is created in addProcessToQueue() using `new Thread(process)`.

2. **Runnable**: When the scheduler calls `currentThread.start()` and the thread is ready to run.

3. **Running**: When the thread is executing the run() method, shown by "▶ P1 executing quantum".

4. **Waiting**: When the thread calls `Thread.sleep()` during the quantum execution to simulate CPU work.

5. **Terminated**: When remainingTime reaches 0 and the process finishes, shown by "✓ P1 finished execution!".

---

## Question 4: Real-World Applications

**Your Answer:**

### Example 1: Web Server

**Description**: 
Web servers handle many user requests at the same time. Each request takes some CPU time to process.

**Why Round-Robin works well here**: 
It ensures no single request hogs the CPU. Even if one request takes a long time, other users still get a response quickly.

### Example 2: Operating System

**Description**: 
Your computer runs many apps at once - browser, music player, text editor.

**Why Round-Robin works well here**: 
The OS gives each app a time slice so everything feels responsive. You can play music while browsing without lag.

---

## Summary

**Key concepts I understood:**
1. Threads are lighter than processes
2. Round-Robin uses time slices for fair scheduling
3. Threads have different states during execution

**Concepts I need to study more:**
1. Thread synchronization
2. Other scheduling algorithms