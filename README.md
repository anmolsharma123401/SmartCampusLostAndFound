#SmartCampusLostAndFound

A Java-based platform designed to streamline the reporting, tracking, and claiming of lost items across a college campus. It replaces physical lost-and-found boards with a centralized system that connects finders with owners.

Key Features

Item Reporting: Log lost or found items with category tags, descriptions, timestamps, and specific campus locations (e.g., Library 2nd Floor, Main Cafeteria).

Smart Search & Filters: Filter records by item category, date range, location, or status (Lost / Found / Claimed).

Automated Match Suggestions: Identifies potential matches between newly logged found items and existing lost reports using basic attribute matching.

Verification & Claiming: Allows users to initiate a claim by providing identifying details only the original owner would know.

Tech Stack & Prerequisites

Language: Java (JDK 17 or higher recommended)

Build Tool: Maven / Gradle

Database: MySQL / PostgreSQL / H2

Framework / UI: Spring Boot / JavaFX / Swing

Getting Started

1. Clone the repository

git clone https://github.com/your-username/SmartCampusLostAndFound.git
cd SmartCampusLostAndFound


2. Configure Database

Update the application properties file (src/main/resources/application.properties or database config class) with your local database credentials:

db.url=jdbc:mysql://localhost:3306/campus_lost_found
db.username=your_username
db.password=your_password


3. Build & Run

Compile and run the project using your preferred IDE (IntelliJ IDEA, Eclipse, VS Code) or the command line:


*How It Works*

Log an Item: A student who lost or found an object submits a report.

Review Matches: The system scans open lost listings against new found listings.

Submit Proof: The claimant submits details verifying ownership.

Resolution: Upon successful verification, the item status updates to Claimed and gets archived.
