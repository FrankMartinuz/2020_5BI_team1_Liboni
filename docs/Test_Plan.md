# **Testing Document and Specification**

*Test Specification*

5BI_Team_1_Liboni


| Client | Server |
| --- | --- |
|Riccardo Radosta | Andrea Liboni |
| Matteo Tognella | Francesco Martino |

## **Client**

### **Incident**

Are listened here the incident discovered while performing various tests on the system

| Incident ID | 2.1-A |
| --- | --- |
| **Description** | To see if the user can see in the interface of the client a table with all the user that are active in that moment |
| **Originator** | Riccardo Radosta |
| **Discover Date** | gg-mm-2019 |
| **Severity** | Medium |
| **Steps Required to Produce Incident** | 1. Go to the page of the login. 2. Click on the bottom of the login. |
| **Cause** | Incident was caused by the code of the software. |
| **Addressed Date** | gg-mm-2019 |
| **Creation Phase** | Implementation |
| **Detection Phase** | Testing |

### **Test**


| Test Case ID: | 2.2 |
| --- | --- |
| **Title** | New user |
| **Feature/Subfeature** | User name and password Validation |
| **Purpose** | To ensure that only passwords with at least one number, one uppercase letter, and at least eight characters long are accepted, |
| **Initial Conditions** | You must be on the "new account" page |
| **Test Data** | Test Data will include invalid passwords like "ciao", "riccardo, 123456789" |
| **Test Actions** | 1. Go to the main page. 2.Click on the button "new user". 3. Insert the data. 4. Click the button "submit"|
| **Expected Results** | With the data that we have used, After Step 4, on the screen must appear an error message, and you must insert a new password (This will happen as long as you insert invalid passwords) |

## **Server**

### **Incident**

| Incident ID | 1.1-A |
| --- | --- |
| **Description** | Missing the creation and starting of a new thread when a user do a second login in the same session. |
| **Originator** | Andrea Liboni |
| **Discover Date** | 12-11-2019 |
| **Severity** | Hard |
| **Steps Required to Produce Incident** | Do a logout from the client and do a re-login in the server whit the same account. |
| **Cause** | Incident was caused by missing check in the code. |
| **Addressed Date** | 14-11-2019 |
| **Creation Phase** | Implementing the multi-threading. |
| **Detection Phase** | Testing |

### **Test**

| Test Case ID: | 1.4-B |
| --- | --- |
| **Title** | Two session at the same time |
| **Feature/Subfeature** | Session validation |
| **Purpose** | Avoid that a user could have at the same time two sesion on two different client |
| **Initial Conditions** | You must have an account and a client |
| **Test Data** | Test Data will include the account information |
| **Test Actions** | You need to open a client, login in the server, and after open another client on the same computer or in another computer in the same network, and try to re-login. |
| **Expected Results** | The server will response with an error message, and inside it Description will be present the error code number 34 (Another session is already open) |
