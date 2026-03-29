# Reflection

## Question 1: What did you learn about multithreading from this assignment?

I learned how to create and manage threads in Java using the Runnable interface. I also learned about the thread lifecycle and how to use methods like start(), join(), and sleep(). The Round-Robin simulation helped me understand how the CPU schedules processes and what happens during context switches. I also learned how to track waiting times and context switches in a real program.

## Question 2: What was the most challenging part of this assignment and why?

The waiting time tracking was the hardest part for me. I had to figure out when processes are actually waiting and when they are running. At first, my waiting time summary showed duplicate processes because the map stored each process multiple times. I spent a lot of time trying to fix this issue.

## Question 3: How did you overcome the challenges you faced?

I fixed the duplicate issue by using a HashMap to store unique processes before printing the summary. For the waiting time calculation, I added timestamps and printed them to understand the flow. I also tested each feature separately and committed my changes after each working feature so I could go back if something broke.

## Question 4: How can multithreading concepts be applied in real-world applications?

Multithreading is used in web servers to handle many users at once without slowing down. It's also used in video games where different threads handle graphics, sound, and user input separately. Another example is media players that use separate threads for video decoding and audio playback so they don't interrupt each other.
