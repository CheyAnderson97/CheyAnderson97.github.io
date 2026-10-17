CS 499 Milestone Three: Artifact Enhancement Narrative
Second Enhancement
Cheyenne "Shay" Anderson
CS 499 Computer Science Capstone
Artifact Title: Project One
Original Course: CS 320: Software Testing, Automation, and Quality Assurance
Professor Maciosek
September 27, 2026


 This artifact continues upon the last enhancement artifact, which contained core classes and service entities. This covered contact, task, and appointment classes and tests. This was originally created in CS 320 and enhanced in the previous milestone. The project uses CRUD operations, input validation, and functions for finding date range overlaps. 
	This artifact was selected because it shows the transition from basic functional java code to thread sage architecture focusing on its data structures and algorithms. The original code relied on sequential collection loops and a mutable state, I would be updating it to show optimization with concurrent execution.
	The components focusing on this weeks category of algorithms and data structure include:
O(1) Hash Map Lookups – these replaced the legacy linear searches (O(n)) with concurrent hash mapping across all service classes, previously it had been added but not fully across all service classes, this enables constant time insertion, deletion, and retrieval of data.
Concurrency and Synchronization: The addition of thread safe updates using “computeIfPresent” and synchronization of critical sections to evaluate time overlap conditions for scheduling under concurrent operations. 
Overlap Algorithm: The appointment conflict detection logic was refactored to evaluate for half open date intervals to prevent scheduling conflicts. 
Several more improvements have been made to this project over the course of these two milestones. The builder pattern has been used across contact, task, and appointment to enforce the immutability during construction. The input validation has been centralized and their rules into AppValidator to decouple the domain state from the assertion logic. As well as added multi thread testing with AppointmentConcurrencyTest which runs 100 parallel threads with ExecutorService and CountDownLatch.
	These updates meet course outcome one employing strategies for software design and execution, as well as course outcome two designing and evaluating computing solutions using appropriate data structures and algorithms. No major revisions to the milestone plan were made or necessary. The refactoring and thread safety goals of module one were again fully realized with the addition of the concurrent testing and immutable patterns in the second enhancement.
	The key takeaways for this enhancement are the immutability combined with the concurrentHashMap that reduced the data corruption and issues from multi thread runtime. As well as delegating the construction to builders isolates validation logic from the management of states. 
	The challenges faced during this enhancement was creating a way to check for overlap while also preventing the overbooking when the threads are made to execute simultaneously, as well as the test harness needing synchronization barriers to force the simultaneous execution and not sequential.
