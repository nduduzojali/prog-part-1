# prog-part-1
Documentation

Design Choices
1.	Architecture: We'll use a three-tier architecture (Presentation, Business Logic, and Data Access) to ensure separation of concerns and maintainability.
2.	Technology Stack: 
Backend: ASP.NET Core 6.0
Frontend: Razor Pages for a server-side rendering approach
Database: SQL Server for robust data management
3.	Authentication: We'll implement ASP.NET Core Identity for secure user authentication and role-based authorization.
Database Structure
The database will consist of the following main entities:
1.	Users: Stores user information (Lecturers, Program Coordinators, Academic Managers)
2.	Claims: Stores claim details submitted by lecturers
3.	Claim Items: Individual line items within a claim (e.g., hours worked, rate)
4.	Documents: Metadata for supporting documents uploaded by lecturers
5.	Claim Status: Tracks the status of each claim
Key relationships:
•	One-to-many between Users and Claims
•	One-to-many between Claims and claim Items
•	One-to-many between Claims and Documents
GUI Layout
The GUI will feature a clean, intuitive design with the following key components:
1.	Dashboard: Personalized view based on user role (Lecturer, Coordinator, Manager)
2.	Claim Submission Form: Easy-to-use form for lecturers to input claim details
3.	Document Upload: Drag-and-drop interface for attaching supporting documents
4.	Claim Status Tracker: Visual representation of claim progress
5.	Approval Interface: Streamlined view for coordinators and managers to review and approve claims
Assumptions and Constraints
1.	Internet Connectivity: Assumes users have reliable internet access
2.	Browser Compatibility: Targets modern web browsers (Chrome, Firefox, Safari, Edge)
3.	Mobile Responsiveness: GUI will be designed with mobile users in mind
4.	Data Privacy: Strict adherence to data protection regulations
5.	Scalability: System should handle up to 1000 concurrent users initially
With this design I aim to create a user-friendly, efficient, and secure system for managing contract lecturer claims, with room for future enhancements and scalability.
