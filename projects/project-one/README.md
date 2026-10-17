CS 499 Milestone Two: Artifact Enhancement Narrative
Course: CS 499 Computer Science Capstone
Author: Cheyenne "Shay" Anderson
Artifact Title: Project One
Original Course: CS 320: Software Testing, Automation, and Quality Assurance 

The original artifact was created as Project One in the CS 320 course (Software Testing, Automation, and Quality Assurance). The original code consisted of three different classes including contact, task, and appointment, along with their service management classes of contactservice, task service, and appointmentservice, as well as several Junit 5 unit tests. The original was designed for basic CRUD operations of create, read, update, and delete of appointments.
	This artifact was included in the ePortfolio because of its demonstration of Java object oriented programming that while contained basic functions, had architectural and performance bottlenecks. Reviewing this artifact showed clear opportunities for demonstration of the improvement of software engineering, algorithm efficiency, and refactoring skills. 
	The specifics of the enhancements made to the project include the following:
Software Engineering & Design Refactoring:
	Centralized Validation replacing repeated validation logic with a single dedicated unity with clear symbolic constants.
	Builder Design Patter refactored instantiation of objects to use the builder pattern to eliminate confusing parameters and guarantee immutability.
	Decoupled Architecture separating data validation, entity representation, and memory layers into distinct modules for DAO patterns.
Algorithmic & Data Structure Optimization:
	O(N) to O(1) Complexity Enhancement replacing linear list searches with indexed data structures (concurrentHashMap)
	Thread safety involved upgrading lookups to constant time speed regardless of dataset size and adding concurrency management without risk of data corruption.
Expanded Unit Testing:
	Updated and refactored Junit 5 testing to validate exception throwing against the new centralized validation utility and builder configurations.

The enhancements completed in this Milestone target the program outcomes in module one. Course outcome three was achieved by transitioning to the concurrentHashMap reducing search time and optimizing memory management and increased transaction. Course outcome 4 was achieved by integrating design patterns (builder, centralized validator, DAO separation) and modernizing code into a scalable architecture. As for major updates and deviations there were no major changes from the roadmap, the only addition was maven software to run the unit testing.
	Reflecting on this project changed my focus of making the code just work to designing software ready for market. This upgrade highlighted how design choice can directly impact the maintainability  and security defense of a program, as well as how using concurrentHashMaps over arrays can demonstrate a payoff between RAM usage and execution safety. The major challenge was refactoring the Junit tests without removing any of the coverage, because the object creation logic had changed with the centralized validation and builders the existing tests failed. This was resolved with updating the tests to use assertations and clauses clean and efficiently.
