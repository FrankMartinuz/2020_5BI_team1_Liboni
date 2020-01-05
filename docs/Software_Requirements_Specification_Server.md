Police Activities League Program Involvement Tracking Project



# *Table of Content*

|1 Introduction|
| --- |
| 1.1 Overview|
| 1.2 Goals and Objectives|
| 1.3 Scope|
| 1.4 Definitions|
| 1.5 Document Conventions|
| 1.6 Assumptions|
| **2 General Design Constraints**|
| 2.1 Product Environment|
| 2.2 User Characteristics|
| 2.3 Mandated Constraints|
| 2.4 Potential System Evolution|
| **3 Nonfunctional Requirements**|
| 3.1 Operational Requirements|
| 3.2 Performance Requirements|
| 3.3 Security Requirements|
| 3.4 Safety Requirements|
| 3.5 Legal Requirements|
| 3.6 Documentation and Training????????????????????????|
| 3.7 External Interface|
| 3.7.1 User Interface|
| 3.7.2 Software Interface|
| **4 System Features**|
| 4.1 Feature: Youth Database|
| 4.1.1 Description and Priority|
| 4.1.2 Use-case: New Registrant|
| 4.1.3 Additional Requirements|
| 4.1.4 Description and Priority|
| 4.1.5 Use-case: Youth Update|
| 4.1.6 Additional Requirements|
| 4.2 Feature: Youth Tracking|
| 4.2.1 Description and Priority|
| 4.2.2 Use Case: Youth Login|
| 4.2.3 Additional Requirements|
| 4.2.4 Description and Priority|
| 4.2.5 Use-case: Youth Logout|
| 4.2.6 Additional Requirements|
| 4.2.7 Description and Priority|
| 4.2.8 Use-case: Administrator comments|
| 4.2.9 Additional Requirements|
| 4.3 Feature: Administrator Access|
| 4.3.1 Description and Priority|
| 4.3.2 Use Case: Administrator Login|
| 4.3.3 Additional Requirements|
| 4.4 Feature: Database Search|
| 4.4.1 Description and Priority|
| 4.4.2 Use-case: Searching the Database|
| 4.5 Feature: Reports|
| 4.5.1 Description and Priority|
| 4.5.2 Use-case: Report Generator|
| 4.5.3 Additional Requirements|
| **5 Appendices**|
| 5.1 Appendix A|
| 5.2 Appendix B|

# 1 Introduction

## 1.1 Overview

This document defines the requirements of the server and client that we develop in the laboratory. For this reason every section will be divded into two part, one for the client and one for the server.  
This document will be useful for the user and for the developer that will need to work on the code.

## 1.2 Objectives
### *Server*
* Develop a server able to make chat client.
* The server will work with different client, but using the same protocol.
* The server have some feature to help the final user in the use of the software.

### *Client*
* punto uno...
* punto due...

## 1.3 Scope

### *Server*
The scope of the server is make communicate an N number of clients between them, and offert at the users some function that can halp, like see the online users and write a brodcast message.
### *Client*


## 1.4 Definitions
definizioni di cose che possono non essere chiare nel documento

### *Server*

### *Client*

## 1.5 Document Conventions

GUI - is the acronym of Graphic User Interface  



TBD – used to indicate information that still needs to be gathered from the customer

Unknown – used to indicate an implementation option that has not yet been decided upon

### *Server*

### *Client*

## 1.6 Assumptions

### *Server*
It is assumed that the client and server are in the same local network, and the firewall is disabled or is integrated a rule that allow the flow of the packet.

# 2 General Design Constraints

## 2.1 Product Environment

### *Server*
The server's software will be put on a server machine, that have to be always active, to permit all the client to connect it and use his services.


The PALPIT software will reside on the central server. Administrators will be able to access the information contained in the database, as well as to generate predefined reports from remote locations. [eeb: good clarification. This is also a section where you could mention that the system will be running in an open area that might be subject to rough treatment. Could also mention that at least one portion will be in an unsecured area.]

## 2.2 User Characteristics

### *Server*
In the server there are no different user, there is only one basic level that allow you to chat with every client online.



**Youth** – Primary and Secondary students with varying computer proficiencies.

**Volunteers** - Adults with computer knowledge sufficient to navigate a web-based interface. These users will be inputting and/or modifying youth registrant information only.

**Administrators** – Adults with computer knowledge sufficient to navigate a web-based interface. These users will be accessing the information and generating reports to assess how the facilities are being used. They will also help the **youth** interact with the system.

## 2.3 Mandated Constraints

### *Server*
The only constraints that we encounter is the obbligation to use the protocol that the professor De Carli gave us, this to make all the communication protocol the same.


There are no constraints at this time. However, there are still key decisions which need to be made (by the customer) which may impose constraints.

## 2.4 Potential System Evolution

### *Server*
At this moment the software of the server is done, but is very basic, so it can be updated in the following ways:
* Add more security control
* Product a log system to keep track of the userm movements.
* Encrypt the message sent in network.





The PALPIT software will most likely be updated in the following ways:

- .Add new activities for youth users to choose from [eeb: will you provide procedure for this until it can be automated?]
- .Add additional youth user information fields (stored in database)
- .Produce new reports

# 3 Nonfunctional Requirements

There are no nonfunctional requirements at this time.

## 3.1 Operational Requirements

There are no operational requirements at this time.

## 3.2Performance Requirements

### *Server*
No requirements for speed have been set forth.  
Memory requirements will be set by the size of the .csv file, that contains all the username and password of the users, but is a simple text file, so it is not relevant.  

## 3.3Security Requirements

There are no security requirements at this time.

## 3.4Safety Requirements

There are no safety requirements at this time.

## 3.5Legal Requirements

There are no legal requirements at this time.

## 3.6 Documentation and Training

The PALPIT documentation will consist of two major portions – one dealing with the administrator features, as well as one dealing with the youth features. Training will be provided to a select group of administrators on administrator _and_ youth features.

## 3.7 External Interface

### 3.7.1 User Interface

#### *Server*
The server have no a GUI, so the only thing you will se on the screen is which computer identify by the IP address is connect at the server.  









Youth Interface-

The youth interface should have a fun interface which will keep the attention of kids long enough for them to enter the following information:

- .Identification (type of identification has not yet been finalized)
- .Whether the user is coming or going
- .Activity the user will be using at the facility

Administrators will need to guide the youth through the &quot;clock-in&quot; procedure at least once and possibly multiple times.

Administrator Interface-

The administrator interface will have a more professional appearance geared towards adults. The interface will provide the following options:

- .Multi-field database query
- .Generate predefined reports
- .Produce custom report

[eeb: good]

### 3.7.2 Software Interface

#### *Server*
See User Interface


# 4 System Features













# 5Appendices

## 5.1Appendix A

Youth Registrant Information

Name

Address

Ethnicity

Age

Sex

School

Student ID #

Date of Birth

Parent Name

Home Phone

Emergency Contact / Phone Number

Medical Insurance Information

Family Physician Name

Family Physician Phone

Hospital Preference

Known Allergies or Medical Conditions

GPA

## 5.2Appendix B

Administrator Options

Multi-field database query

Generate predefined reports

Generate custom reports

Update Youth Record

TBD
