# Operating-Platforms-2026

Professional Portfolio Overview:

This portfolio presents selected work from Operating Platforms 2026. The materials show growth in operating system concepts, object-oriented design, client-server architecture, REST APIs, security, memory management, storage management, and distributed-system recommendations. The work is organized so it can support a GitHub profile, repository README, course reflection, and job-readiness portfolio.
Career goal: apply computer science and electrical engineering knowledge toward technical work in the space industry, including computer engineering technician or satellite engineering technician roles.
Repository description: CS 230 Operating Platforms portfolio: OS analysis, software 	design, Java singleton application, REST API security, memory/storage planning, and 	final recommendations

# Operating Systems Discussion

Compared Windows and Android, described daily OS use, and connected computer science goals to engineering and future technical work.
Object-Oriented and UML Foundations:
Explained encapsulation, inheritance, abstraction, constructors, getter/setter methods, and relationships in a UML class diagram.
Software Design and Singleton Project: 
Created and reviewed a Java design for The Gaming Room using a GameService singleton to manage unique game instances.
Client-Server Architecture and REST APIs:
Explained separation of client and server responsibilities, REST endpoints, platform independence, database interaction, and support for future clients.
Security Across Operating Platforms:
Discussed authentication, authorization, role-based access control, least privilege, encryption, patching, logging, monitoring, and secure design.
Memory, Storage, and Distributed Systems:
Analyzed active memory needs, image caching, permanent storage, database uniqueness, cloud/file storage, backups, and scalability.

# Featured Project-1: Draw It or Lose It Java Application

The Java project demonstrates object-oriented design and the singleton design pattern. The GameService class controls creation of game objects and prevents duplicate game names by returning the existing object when a name already exists. This supports the client requirement that only one instance of a game service should exist in memory.
•	Language and tools: Java, Eclipse, UML, object-oriented design.
•	Core classes: GameService, Game, Team, Player, SingletonTester, and ProgramDriver.
•	Main pattern: singleton pattern for central management of game objects.
•	Key requirement supported: unique game identifiers and prevention of duplicate game names.
•	Portfolio message: demonstrates ability to translate design requirements into working Java code.

## Client and Software Requirements Summary

The client for this project was The Gaming Room, a company that already had an Android game called Draw It or Lose It. The company wanted to expand the game from an Android-only application into a web-based, multi-platform application that could support users on Windows, macOS, Linux, Android, iOS, and browser-based environments. The requested software design needed to preserve the game rules while supporting multiple games, teams, and players, enforcing unique game and team names, and using a controlled service layer to manage game creation.

Key requirements included:

•	Support one or more games, with each game containing one or more teams.
•	Allow each team to contain multiple players while preventing duplicate player names within a team.
•	Enforce unique game names and unique team names so users can know whether a name is already in use.
•	Use a single GameService instance in memory through the singleton design pattern.
•	Assign unique identifiers to games, teams, and players.
•	Prepare the software for future distributed, web-based, and multi-platform deployment.
•	Support future security, persistence, REST API, and database integration as the application grows.

## Strength in developing the documentation

I did particularly well organizing the client requirements into a clear software design plan. The documentation connects the client’s business goal with specific technical decisions, including the domain model, inheritance structure, singleton GameService pattern, and recommendations for a Linux-based server platform. I also explained why the design supports future expansion to multiple platforms instead of keeping the product limited to Android.

## Helpful Parts of the Design Document Process

The design document was helpful because it created a roadmap before coding began. By identifying the required objects, relationships, constraints, and design patterns first, the code became easier to plan and test. For example, the need for unique games, teams, and players led directly to search logic before creating new objects. The requirement for one service instance led directly to the singleton GameService design. This process reduced confusion because the code was tied back to documented client needs.

## Area I would Revise

If I could revise one part, I would improve the system architecture section by adding a more detailed deployment view. The current design explains the logical direction of a layered web architecture, but a stronger version would include a diagram showing the browser or mobile client, REST API, application service layer, database, authentication service, and cloud-hosted Linux server. This would make the transition from the current prototype to a production-ready distributed system easier for both the client and the development team to understand.

## Interpreting User Needs in the Software Design

I interpreted the user’s needs by focusing on how players, teams, and games would actually interact with the system. The Gaming Room needed a design that would prevent duplicate game and team names, support multiple teams and players, and allow the application to grow beyond one operating system. Those needs were implemented through object-oriented classes, shared Entity fields, composition relationships, and a singleton service class that manages game creation. Considering user needs is important because software is successful only when it solves the real problem for the client and end users. If user needs are ignored, the application may technically run but fail to provide the correct experience, security, scalability, or usability.

## Approach to Designing Software

I approached the design by first studying the client’s requirements, then identifying the main entities, relationships, and constraints. I used object-oriented design to separate responsibilities among Game, Team, Player, Entity, and GameService. I also used design patterns, especially the singleton pattern, to solve the requirement that only one game-management service should exist in memory. In the future, I would continue using requirements analysis, UML diagrams, layered architecture, pseudocode, design patterns, and early testing. I would also add more security and database planning earlier in the process so the prototype can transition more smoothly into a production web application.

## References

Oracle. (n.d.). Java Platform, Standard Edition documentation. https://docs.oracle.com/en/java/javase/
Oracle. (n.d.). The Java Tutorials: Object-oriented programming concepts. https://docs.oracle.com/javase/tutorial/java/concepts/
Refactoring.Guru. (n.d.). Iterator. https://refactoring.guru/design-patterns/iterator
Refactoring.Guru. (n.d.). Singleton. https://refactoring.guru/design-patterns/singleton
The Gaming Room. (2026). Draw It or Lose It CS 230 project software design template [Unpublished course project].
The Gaming Room. (2026). GameAuth Maven source project [Unpublished source code archive].
