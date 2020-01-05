## 4.1 Feature: Youth Database

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
