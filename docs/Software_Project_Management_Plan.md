
# Software Project Management Plan

**Project Name** ServerClientChat

**Date of last change** 12/11/2019

**Team Members**
Liboni Andrea
Tognella Matteo
Radosta Riccardo
Martino Francesco

**Document Control**

Change History
| Revision | Change Date | Description of changes |
|:-:|:-:|:-:|		
| V1.0 | 22/10/2019 | Initial release |

**Document Storage**
This document is stored in the project’s SVN repository at: https://github.com/FrankMartinuz/2020_5BI_team1_Liboni.

**Document Owner**
Martino Francesco is the owner of the repository.

**Table of Contents**

***1 OVERVIEW***
1.1	Purpose and Scope
1.2	Goals and Objectives
1.3	Project Deliverables
1.4	Assumptions and Constraints
1.5	Schedule and Budget Summary
1.6	Success Criteria
1.7	Evolution of the Project Plan
***2 STARTUP PLAN***
2.1	Team Organization
2.2	Project Communications
2.3	Technical Process
2.4	Tools
***3 WORK PLAN***
3.1	Activities and Tasks
3.2	Release Plan
3.3	Budget
***4 CONTROL PLAN***
4.1	Monitoring and Control
***5 SUPPORTING PROCESS PLANS***
5.1	Risk Management Plan
5.2	Configuration Management Plan
5.3	Verification and Validation Plan

## 1	Overview
### 1.1	Purpose and Scope

**Server**
The purpose of this project is to give a kind of text messaging application.
The scope oh the server is manage some requests from the clients. This requests can be arequest for see a list of online users, and a request for send a text-message to one, or more, online users.

### 1.2	Goals and Objectives

**Server**
The overall goal is to give students a method to chat with their classmate. The app is expected to:

* Manage the user identification through the sign in, log in and log out

* Provide a way to chat with class members.

* Give to client a server that can manage all request.

* Guarantee to every client a reply in useful time.

### 1.3	Project Deliverables

**Server**
The following items will be delivered to the customer on or before 6/1/2020:
1.	Source code for both the client and server portions of the system.
2.	User’s Guide
3.	Project Charter
4.	Software Requirements Specification
5.	Software Project Management Plan
6.	Business Model Canvas
7.	Project Model Canvas

### 1.4	Assumptions and Constraints

**Server**
Assumptions:
1.	The protocol will always work
2.	The server will always send a feedback about the request. (Done or Failed)
Constraints:
1.	The server must follow the teacher protocol
2.	The server must be on the school LAN for work.
3.	The server must be ready by 12/11/2019.

### 1.5	Schedule and Budget Summary

**Server**
Schedule:
29/10/2019 - Create the file system of the program and planned the job
29/10/2019 - Add private message function and user vector
29/10/2019 - End the main part of the software
05/11/2019 - Testing
05/11/2019 - Fixing the problems and bugs issue during the test
05/11/2019 - End the software development
20/11/2019 - Begin the documentation

Budget:
There are not production costs, in terms of money. We have only spend an a amount of 4 lesson at school.
3 (hours for lesson) * 4 (lessons) = 12 total hours

### 1.6	Success Criteria

**Server**
The project will be a success if:
* It work without bugs and problems with all the different client that our classmate have done and in all the situation that we expected.
* It is ready before the delivery date.

## 2	Startup Plan
### 2.1	Team Organization

**Server**
Teacher: Provide to us a packs protocol that we have to use in our chat.
Programmers (2): Programmers have to plan the project, and after write all the code.

### 2.2	Project Communications

**Server**
For share our code and all the information we have used GitHub.
For the verbal communication we simply talk in classroom.

### 2.3	Technical Process

**Server**
For this project we have proceeded step by step.
The first step was create a listening server. Successively every packet-request available stand for one steps.
In this way we were sure that when we pass one step, the latter did not have bugs.

### 2.4	Tools

*	Programming Language – Python
*	Version Control – source code and written artifacts will be stored in a GitHub repository.
* Packs protocol - invented and supplied by our teacher


## 3	Work Plan
### 3.1	Activities and Tasks

**Server**
Every tasks, except the first ("create a server"), take the name from the type of packets analyzed.
At the end of all steps, there are many testing activities, using some testing clients created by us.

### 3.2	Release Plan

**Server**
For this project we have choosen to do only one release, or rather the final release.
This choice born because this is project have limited size and features.

### 3.3	Budget

**Server**
For every steps we spent about an half hour.
For the testing and bug fixing we have used about 2 hours.
We haven't costs in terms of money.

## 4	Control Plan
### 4.1	Monitoring and Control

**Server**
01-10-2019 - Study of protocols
15-10-2019 - Study of sockets
22-10-2019 - Undestand chat's protocols
29-10-2019 - Start programming in Python.
12-11-2019 - Deliver the functioning server

## 5	Supporting Process Plans
### 5.1	Risk Management Plan
**Server**
One risk, that the final user can spot in this software, is the overload of the LAN, or of the Computer where the server is running.
This problem depends, first of all, on power of the PC where the server has been ran, in second on how many clients want to use the service simultaneously. The only way to fix this problem is to improve the PC stats, or increase the band available.

5.2	Configuration Management Plan
Configuration management plans for this document and other baselined work products including review procedures and change management procedures.

Partial Example
1.	All work products will be stored in a centralized CVS repository running on a central server.
2.	The naming convention for documents will be: NNN-VVV.suffix  where NNN is a mnemonic that reflects the function of the document, VVV is a 3 digit version number, and 'suffix' is the standard/normal suffix for the document type. For example, the second version of the requirements document created as a Microsoft Word document might be labeled: REQ-002.doc.
3.	All project (work products) items (documents, source code, test cases, program data, test data, etc) will be stored in the CVS repository but not all will be under change control (subject to formal change control procedures.) Only the system requirements, project plan and source code will be baselined and under configuration control.
4.	Items that are subject to change control will be considered baselined after a group review at the end of the life cycle phase during which they are created. Baselined here means that the product has undergone a formal review and can only be changed through the prescribed change control procedures.
5.	The change control procedure once a product is baselined is: (1) anyone wanting to make a change to a baselined item sends an email to the rest of the group describing the change, reason for the change, expected impact, and timeline for integrating the change. (2) if no one responds to the group within 2 days with a reason for why the change request shouldn't be permitted, it will be considered accepted and the person proposing the change may proceed with the change. If anyone does object to the change, the reason for objecting will be discussed at a meeting where everyone is invited to attend and voice their opinion. At the end of the meeting a democratic vote will be held to decide whether or not the change should be allowed.
6.	Including a change history with all documents is encouraged but only required for baselined documents. The change history should be at the front of the work item and include: (1) the name of the person making the change, (2) brief description of what has changed, (3) reason for the change, and (4) the date the change was integrated.

5.3	Verification and Validation Plan
The verification and validation plan defines what actions are being taken to assure the quality of the development process and resulting software products.

Partial Example
The Verification and Validation plan is specified as a separate documented located in the version control system at: http://company.com/svn/project-name/docs/VandVPlan.doc

5.4	Product Acceptance Plan
The product acceptance plan defines what is acceptable in terms of product quality and product functionality. Acceptance criteria should be objective and measurable. Note product success is one aspect of project success.  Teams wanting to establish a clear understanding of what will be considered acceptable project performance may want to define a more general plan for project success that includes quantitative goals for delivery date, cost, etc.

Partial Example
The Verification and Valida


SEI UN TARDO
