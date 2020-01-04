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
| 3.6 Other Quality Attributes|
| 3.7 Documentation and Training|
| 3.8 External Interface|
| 3.8.1 User Interface|
| 3.8.2 Software Interface|
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
The scope of the server is 








PALPIT will provide the ability to store information about youth users of PAL facilities in a database which will be searchable on any field. PALPIT will also provide the ability to track the use of PAL facilities by registered youth users and store this information in a database.









## 1.4Definitions

(this section will be expanded in later versions)

**Use case** – describes a goal-oriented interaction between the system and an actor. A use case may define several variants called scenarios that result in different paths through the use case and usually different outcomes.

**Clock-in** – time at which a youth participant begins to use a PAL facility

**Clock-out** – time at which a youth participant exits a PAL facility

**Registered Youth** – a PAL facility user who has a record in the youth database

**Registrant** – (see &quot;Registered Youth&quot;)

**Youth Database –** where information about registered PAL facility users is stored

**PAL** – Police Activity League

**PALPIT** – Police Activity League Program Involvement Tracking Program

## 1.5Document Conventions

TBD – used to indicate information that still needs to be gathered from the customer

Unknown – used to indicate an implementation option that has not yet been decided upon

## 1.6Assumptions

It is assumed that all three PAL facilities will have browser based access to a central server.

# 2General Design Constraints

## 2.1Product Environment

The PALPIT software will reside on the central server. Administrators will be able to access the information contained in the database, as well as to generate predefined reports from remote locations. [eeb: good clarification. This is also a section where you could mention that the system will be running in an open area that might be subject to rough treatment. Could also mention that at least one portion will be in an unsecured area.]

## 2.2User Characteristics

**Youth** – Primary and Secondary students with varying computer proficiencies.

**Volunteers –** Adults with computer knowledge sufficient to navigate a web-based interface. These users will be inputting and/or modifying youth registrant information only.

**Administrators** – Adults with computer knowledge sufficient to navigate a web-based interface. These users will be accessing the information and generating reports to assess how the facilities are being used. They will also help the **youth** interact with the system.

## 2.3Mandated Constraints

There are no constraints at this time. However, there are still key decisions which need to be made (by the customer) which may impose constraints.

## 2.4Potential System Evolution

The PALPIT software will most likely be updated in the following ways:

- .Add new activities for youth users to choose from [eeb: will you provide procedure for this until it can be automated?]
- .Add additional youth user information fields (stored in database)
- .Produce new reports

# 3Nonfunctional Requirements

There are no nonfunctional requirements at this time. [eeb: au contraire, usability, maintainability (talk to the pharmacy teams this semester if you don&#39;t think maintainability is a non-functional requirement),]

## 3.1Operational Requirements

There are no operational requirements at this time.

## 3.2Performance Requirements

No requirements for speed have been set forth.

Memory requirements will be nominal (exact size is not known at this time) as the database will be holding information for approx. 200 people. Queries on this database should take no more than 4 seconds.

## 3.3Security Requirements

Only one type of user will have access to the database information. Therefore, only one user level is needed. The database will hold some confidential information about the youth who use the PAL facilities. Only users who are authorized to see the information should have access to it.

## 3.4Safety Requirements

There are no safety requirements at this time.

## 3.5Legal Requirements

(See security requirements)

## 3.6Other Quality Attributes

There are specific sections above for non-functional quality attributes such as security, performance, etc. In this section describe any other non-functional quality attributes such as portability, availability, etc.

## 3.7Documentation and Training

The PALPIT documentation will consist of two major portions – one dealing with the administrator features, as well as one dealing with the youth features. Training will be provided to a select group of administrators on administrator _and_ youth features.







## 3.8External Interface

### 3.8.1User Interface

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

### 3.8.2Software Interface

Unknown.

# 4System Features

## 4.1Feature: Youth Database

The Youth Database will be where all of the information about the users of the PAL facilities will be kept. This section describes how new registrant information will be added to the database.

### 4.1.1Description and Priority

The New Registrant process allows a volunteer or administrator to add an unregistered youth to the database.

Cost: medium

Risk: low

Value: high

### 4.1.2Use-case: New Registrant

**Actors:** volunteer or administrator

**Description:** The use-case begins when an unregistered youth submits a registration form (hard copy). It is assumed that the administrator or volunteer has already completed the login process.

Basic Path:

1. The user will be prompted to enter all of the information found in Appendix A
2. The user will enter _at least_ the information which is required to register
3. The information will be recorded in the database and acknowledgement sent back to the user.

Alternate Path:

1. If step 2 is unsuccessful the user will see an error message on screen indicating what information still _needs_ to be provided
2. The user will then be prompted to go back and fill out the remaining required items
3. The user now returns to step 2 of the &quot;Basic Path&quot;

### 4.1.3Additional Requirements

N/A

### 4.1.4Description and Priority

The Youth Update process allows an administrator to modify or delete any information in a registrant&#39;s record.

Cost: medium

Risk: low

Value: medium

### 4.1.5Use-case: Youth Update

**Actors:** administrator

**Description:** The use-case begins when after the user has logged in to the administrator interface and wishes to update a registrant&#39;s information.

Basic Path:

1. The user will navigate to the youth update page
2. The user will be prompted to enter the name of the person whom they will be updating information on
3. The user will be presented with all information about the registrant stored in the database
4. The user will be able to modify any of the information
5. The user will enter changes into the appropriate fields
6. The user will submit the changes
7. The system will update the registrant&#39;s record

### 4.1.6Additional Requirements

The administrator will be able to add a new registrant or delete a current registrant.

## 4.2Feature: Youth Tracking

The Youth Tracking portion of the software will allow administrators to keep track of how much time registered participants use the facilities, as well as how they use the facilities (i.e. what activities they participate in).

### 4.2.1Description and Priority

The Youth Login Screen Access will allow an administrator or volunteer to bring up the youth login screen.

### 4.2.2Use Case: Youth Login Screen Access

**Actors:** administrators or volunteers

**Description:** The use case begins when an administrator or volunteer wants to display the youth login screen.

Basic Path:

1. User opens a web browser and navigates to the web-interface of the system
2. User will choose the &quot;Youth Login Screen&quot; option from a list
3. System will prompt user for a username and password
4. User will enter username and password
5. System will verify username and password
6. Youth Login Screen will be displayed

Alternate Path:

1. if step 5 fails user will be notified that the username or password entered was incorrect
2. user will be prompted to reenter username and password
3. return to step 5 of basic path
4. if login fails 3 times user will be prompted to have their password sent to their email address

### 4.2.3Additional Requirement

N/A

### 4.2.4Description and Priority

The Youth Login will gather the following information:

- .Identification information
- .Time the user begins using the facility
- .What activity the user will be using

Cost: medium

Risk: low

Value: high

### 4.2.5Use Case: Youth Login

**Actors:** Registered Youth

**Description:** The use-case begins when the registered youth enters the PAL facility to participate in an activity.

Basic Path:

1. User is prompted to provide identification to the system
2. User provides identification to system
3. System verifies the identification. If the id is verified the system will store the current time as the user&#39;s &quot;clock-in&quot; time.
4. System prompts user to select which activity they will be participating in
5. User selects which activity (or activities) they will be participating in
6. System stores the activity and notifies user of successful login
7. System returns to Youth Login Screen automatically

Alternate Path:

1. If step 3 is not completed this indicates that the system does not recognize the user&#39;s identification information. The system will prompt the user to retry inputting the identification information. If retry is successful use-case resumes at step 4 of &quot;Basic Path&quot;. If retry is unsuccessful use-case proceeds to step 2 of &quot;Alternate Path&quot;.
2. System notifies the user that they are not recognized by the system and, therefore, will require assistance from an administrator.
3. Return to step 7 of basic path

### 4.2.6Additional Requirements

N/A

### 4.2.7Description and Priority

The Youth Logout will store the time that the registered youth participant leaves the PAL facility.

Cost: low

Risk: low

Value: high

### 4.2.8Use-case: Youth Logout

**Actors:** Registered youth who have been using a PAL facility

**Description:** The use-case begins when the registered youth finishes participating in an activity at a PAL facility.

Basic Path:

1. System prompts user for identification information
2. User provides identification information to system and indicates to the system that they are clocking out
3. System verifies that the user is currently clocked-in
4. Upon verification system stores the clock-out time and notifies user of successful clock-out
5. System returns to Youth Login Screen automatically

Alternate Path:

1. If step 3 is not completed this indicates that the user never clocked in.
2. System will prompt the user to select which activity (or activities) they have been using
3. User selects which activity (or activities) they have been using
4. System stores this information and notifies user of successful clock-in
5. Return to step 5 of basic path

### 4.2.9Additional Requirements

If a user fails to clock out, the system will automatically store the closing time of the facility as the user&#39;s clock out time. Administrators will have the ability to edit clock-out times if needed. [eeb: good]

### 4.2.10Description and Priority

The administrator will be able to add comments to the record of a registered youth participant.

Cost: low

Risk: low

Value: medium

### 4.2.11Use-case: Administrator comments

**Actors:** administrators

**Description:** The use case begins after the administrator has logged in and wishes to add a comment to the record of a registered youth.

Basic Path:

1. The user will navigate the administrator user interface to the page that prompts the user to identify the registered youth they wish to comment on
2. The user will identify the youth they intend to comment on
3. The user will be prompted to enter the comment
4. The user will enter and submit the comment
5. The system will store the comment in the youth&#39;s record

### 4.2.12Additional Requirements

N/A

## 4.3Feature: Administrator Access

### 4.3.1Description and Priority

The Administrator Access feature will provide a means to access the information stored in the database.

Cost: low

Risk:  medium

Value: high

### 4.3.2Use Case: Administrator or Volunteer Login

**Actors:** administrators

**Description:** The use case begins when the user decides to access the administrator or volunteer functions of the system.

Basic Path:

1. The user will open up the web-interface of the system in a web browser
2. The user will navigate to the login page
3. The system will prompt the user for user name and password
4. User will provide user name and password
5. System will verify user name and password
6. The user will be presented with the options listed in Appendix B

Alternate Path:

1. If step 5 is unsuccessful the system will notify the user that the login attempt failed
2. The user will be prompted to retry the login
3. If the login attempt fails the user will be given one more opportunity to login in
4. If step 3 fails the user will be prompted to have their password sent to their email address
5. Upon approval by the user the password will be sent to the user&#39;s email address

### 4.3.3Additional Requirements

N/A

## 4.4Feature: Database Search

### 4.4.1Description and Priority

The Database Search feature will allow administrators to search the database by any of the information fields in the youth registrant records.

Cost: medium

Risk: medium

Value: medium

### 4.4.2Use-case: Searching the Database

TBD

## 4.5Feature: Reports

### 4.5.1Description and Priority

The Report Generator will produce predefined and custom reports for administrators.

### 4.5.2Use-case: Report Generator

TBD

### 4.5.3Additional Requirements

N/A



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
