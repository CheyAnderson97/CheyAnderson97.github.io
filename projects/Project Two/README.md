
CS 499 Milestone Four: Artifact Enhancement Narrative
Third Enhancement
Cheyenne "Shay" Anderson
CS 499 Computer Science Capstone
Artifact Title: Project Two
Original Course: CS 340 Client/Server Development
Professor Maciosek
October 4, 2026


 The artifact I selected for this enhancement is the Animal Shelter Dashboard and CRUD Python Module of project two in the CS 340 course. It creates a Python database module that uses MongoDB. With a Plotly Dash web dashboard that would allow users to filter the records of shelter animals by the rescue type, and then visualize these results on a interactive table and map. This was created very early in this year and has been improved and updated for this course.
This project was selected as it demonstrates a full stack data driven application that shows the bridge between back end database operations and an interactive web base front end. It is a comprehensive showing of database management, object oriented designs, software testing, and interactive user interface development. Some specific components include:
•	Database interface and design- AnimalShelter class encapsulates PyMongo CRUD operations, and enforces proper error and exception management for the database.
•	Interactive UI/UX- Jupyter Dash interface creates integration between custom widgets, data tables, and map components, which allow filtering and location rendering based on interactions from the user.
•	CI/CD Workflows- Including GitHub Actions shows modern software integration and includes automatic testing and integration.
	Many improvements were made to this piece in this enhancement. I expanded and added thorough exception handling across the database queries to help prevent unhandled runtime errors. The callback Dash logic was refactored for improved response and cleaner state management when the map markers and data tables view’s are updated. As well as refining the testing scripts to make sure full coverage of database interactions.
	The enhancement of this project meets the planned course outcomes from module one. In reference to software design and engineering the software architecture was improved by decoupling the UI elements from the data layer access and the addition of modular components. Next, algorithms and data structures were enhanced with added data filtering and pipelines added to feed the ploty dash data table map coordinates efficiently. And lastly, databases, these were refactored through schema queries and PyMongo driver calls to make sure the program is secure and has optimized execution.
	No major updated happened from the initial plan of enhancement, additions were added with the integration testing with GitHub Actions to improve code quality and reliability of the build.
	Enhancing this project helped me to learn more about redesigning legacy code and helped to highlight the importance of API boundaries between data access layers and front end state management. I also gained more knowledge of geo coordinate data dynamic updates in maps with Dash callbacks. This knowledge helped me to advance my skills and overcome challenges like ensuring the synched updates of the Dash data table and the Leaflet map markers. The other issue I encountered during this is during testing phase I kept receiving warnings about the secret key I created only being 11 bytes long but these were no longer occurring when I generated a 32 byte key and updated it in the program. 
