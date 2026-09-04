# PROG6212POEPART1
RaceDay — Part 1

RaceDay is a web-based event management system for South African road running, walking and cycling events.

Part 1 documents

All Part 1 planning documents are stored in /docs:

• RaceDay_ERD.png — Entity Relationship Diagram
• API_Endpoint_Plan.md — REST API endpoint plan
• RaceDay_Database.sql — SQL Server database script
• RaceDay_ERD.dot — editable Graphviz source for the ERD

Database setup

1. Open SQL Server Management Studio (SSMS).
2. Open docs/RaceDay_Database.sql.
3. Run the complete script on a clean SQL Server instance.
4. Confirm that the tables and sample records are created without errors.
5. The script creates RaceDayDb if it does not already exist.

ERD and implementation

The SQL database is designed to match the ERD. The main relationships are:

• One organiser can organise many events.
• One participant can have many enrolments.
• One event can have many categories.
• One event can have many enrolments.
• One category can have many enrolments.
• One enrolment can have zero or one result.
• One event can have zero or one route.
• One event can have many weather snapshots.
