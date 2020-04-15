**Testing Document and Specification**

Test Specification

5BI_Team_1_Liboni


| Client | Server |
| --- | --- |
|Riccardo Radosta | Andrea Liboni |
| Matteo Tognella | Francesco Martino |

**Client**

**Incident**

Are listened here the incident discovered while performing various tests on the system

| Incident ID | 2.1-A |
| --- | --- |
| Description | To see if the user can see in the interface of the client a table with all the user that are active in that moment |
| Originator | Riccardo Radosta |
| Discover Date | gg-mm-2019 |
| Severity | Medium |
| Steps Required to Produce Incident | 1. Go to the page of the login. 2. Click on the bottom of the login. |
| Cause | Incident was caused by the code of the software. |
| Addressed Date | gg-mm-2019 |
| Creation Phase | Implementation |
| Detection Phase | Testing |

**Test**


| Test Case ID: | 2.2 |
| --- | --- |
| Title: | New user |
| Feature/Subfeature: | User name and password Validation |
| Purpose: | To ensure that only passwords with at least one number, one uppercase letter, and at least eight characters long are accepted, |
| Initial Conditions: | You must be on the "new account" page |
| Test Data: | Test Data will include invalid passwords like "ciao", "riccardo, 123456789" |
| Test Actions: | 1. Go to the main page. 2.Click on the button "new user". 3. Insert the data. 4. Click the button "submit"|
| Expected Results: | With the data that we have used, After Step 4, on the screen must appear an error message, and you must insert a new password (This will happen as long as you insert invalid passwords) |

**Server**

**Incident**

Are listened here the incident discovered while performing various tests on the system

| Incident ID | 2.1-A |
| --- | --- |
| Description | Inventa quacosa, se vuoi vedere un esempio non modificato guarda il file 27.doc (dagli un occhiata perche io ho cancellato anche qualche riga nella tabella degli incident) |
| Originator | Riccardo Radosta |
| Discover Date | gg-mm-2019 |
| Severity | Medium |
| Steps Required to Produce Incident | 1. Go to the page of the login. 2. Click on the bottom of the login. |
| Cause | Incident was caused by the code of the software. |
| Addressed Date | gg-mm-2019 |
| Creation Phase | Implementation |
| Detection Phase | Testing |

**Test**
Ti ho lasciato un tre esempi sotto, il primo è il mio, gli altri sono loro, se ne vuoi ancora vai a vedere il file 25.doc

| Test Case ID: | 2.2 |
| --- | --- |
| Title: | New user |
| Feature/Subfeature: | User name and password Validation |
| Purpose: | To ensure that only passwords with at least one number, one uppercase letter, and at least eight characters long are accepted, |
| Initial Conditions: | You must be on the "new account" page |
| Test Data: | Test Data will include invalid passwords like "ciao", "riccardo, 123456789" |
| Test Actions: | 1. Go to the main page. 2.Click on the button "new user". 3. Insert the data. 4. Click the button "submit"|
| Expected Results: | With the data that we have used, After Step 4, on the screen must appear an error message, and you must insert a new password (This will happen as long as you insert invalid passwords) |

| Test Case ID: | 4.1.2.1 |
| --- | --- |
| Title: | Submitting a Question |
| Feature/Subfeature: | Asking Questions |
| Purpose: | To ensure that valid users are able to submit questions that they would like answered. |
| Initial Conditions: | Current user must be on the &quot;Ask a Question&quot; page, which means that they have already been authenticated as a valid user. |
| Test Data: | Category: Injuries Title: When to see a doctorQuestion: Should I go see the doctor if I have cut my finger and it will not stop bleeding? |
| Test Actions: | 1. From the &quot;Ask a Question&quot; page select Injuries from the categories drop down menu2. Enter test data title in the &quot;Title&quot; text box3. Enter test data question in the &quot;Question&quot; text box4. Select &quot;Submit Question&quot; button |
| Expected Results: | After step 4, a thank you message should appear, thanking the user for submitting a question. User should then be asked to view previously asked questions. Question should appear on back end site for provider discussion.Note: Question will not appear on main question page until answer has been submitted. |

| Test Case ID: | 4.1.2.2 |
| --- | --- |
| Title: | Submitting a Question with Special Characters |
| Feature/Subfeature: | Asking Questions |
| Purpose: | To ensure that valid users are able to submit questions that they would like answered and to make sure special characters do not cause problems with question submission and data validation. |
| Initial Conditions: | Current user must be on the &quot;Ask a Question&quot; page, which means that they have already been authenticated as a valid user. |
| Test Data: | Category: Injuries Title: When to see a doctorQuestion: &quot;Should I go see the doctor if I have cut my finger and it will not stop bleeding?@#$%&quot; |
| Test Actions: | 1. From the &quot;Ask a Question&quot; page select Injuries from the categories drop down menu2. Enter test data title in the &quot;Title&quot; text box3. Enter test data question in the &quot;Question&quot; text box4. Select &quot;Submit Question&quot; button |
| Expected Results: | After step 4, a thank you message should appear, thanking the user for submitting a question. User should then be asked to view previously asked questions. Question should appear on back end site for provider discussion.Note: Question will not appear on main question page until answer has been submitted. |
