Prompt:
This is a multithreaded Java program that uses synchronized methods (reentrant locks or semaphores) to control access to a one-
lane bridge. One thread should simulate westbound vehicles and another thread should simulate eastbound vehicles. The vehicles 
do not have a reverse gear, so the bridge would become deadlocked if both a westbound vehicle and an eastbound vehicle were 
allowed to drive onto the bridge at the same time. Therefore, mutual exclusion must be enforced on the use of the bridge. 
The solution will avoid both deadlock and starvation. Vehicles traveling in either direction should wait (sleep) for some amount
of time, then attempt to cross. Once a vehicle is on the bridge, it will sleep to simulate crossing the bridge. There will be
a message when each vehicle drives onto the bridge and another message when that vehicle has completed the crossing. 
