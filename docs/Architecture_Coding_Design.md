[Project Name]
Architecture/Design Document


Table of Contents
1. INTRODUCTION
2.	DESIGN GOALS
3.	SYSTEM BEHAVIOR
4.	LOGICAL VIEW	  
.1	High-Level Design (Architecture)
.2	Mid-Level Design
.3	Detailed Class Design
5.	PROCESS VIEW
6.	DEVELOPMENT VIEW
7.	PHYSICAL VIEW
8.	USE CASE VIEW


Change History  
Version: <1.0>  
Modifier: <First version>  
Date: 12/11/2019  
Description of Change: First release of complete application
______________________________________________________

#	Introduction

**Server**

This document describes the architecture and design for the ServerChat application being developed for De Carli Lorenzo.

With this server every group's member can chat with another classmate. The advantage of this system is that it's more secure because it's working only on the LAN

The purpose of this document is to describe the architecture and design of the ServerChat application in a way that addresses the interests and concerns of all major stakeholders. For this application the major stakeholders are:

•	Users and the customer – they want assurances that the server will provide a service simple but that it works well for resttrict use that it will have
•	Developers – they want an architecture that will minimize complexity and development effort.
•	Project Manager – the project manager want a clean work, as simple as possible. They also want a clear everyone's knowledge of the whole project
•	Maintenance Programmers – they want assurance that the system will be easy to modify in case of bugs.

#	Design Goals

**Server and Client**

The design priorities for the ServerClientChat application are:
•	The design should minimize complexity and development effort.
•	The design should be easy to modify from every programmer.
• The design must be follow the PEP-8 coding standards

#	System Behavior
The use case view is used to both drive the design phase and validate the output of the design phase. The architecture description presented here starts with a review of the expect system behavior in order to set the stage for the architecture description that follows. For a more detailed account of software requirements, see the requirements document.

<brief description of system behavior>

4	Logical View
The logical view describes the main functional components of the system. This includes modules, the static relationships between modules, and their dynamic patterns of interaction.

In this section the modules of the system are first expressed in terms of high level components (architecture) and progressively refined into more detailed components and eventually classes with specific attributes and operations.
4.1	High-Level Design (Architecture)
The high-level view or architecture consists of <?> major components:

<list and/or show major architecture components>

Example:
System Architecture
•	The GPS device provides the user’s location on campus (longitude and latitude coordinates). In basic mode, the user’s position is used to decide which buildings to announce.
•	The Database is a central repository for data on buildings, their locations and associated audio segments.
•	The Audio Player controls playback of audio files.
•	Given a position on earth, the Mapping Logic will calculate nearby buildings.
•	The Application Control Logic is the main driver of the application. It presents information to the user and reacts to user inputs.
4.2	Mid-Level Design
<Explain and/or show static and dynamic aspects of subsystem components. Probably the most effective way of showing mid-level design is with class and sequence diagrams.>
4.3	Detailed Class Design
<For a few key classes you might want to show associations, attributes and methods.>

5	Process View

<Where are the threads of control in the application?>


6	Physical View
<Where will major components be physically deployed?>
7	Use Case View
<Sketch architecturally significant use cases.>
