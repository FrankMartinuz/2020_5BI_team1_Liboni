# **Test Case Specification**

April 17, 2020

Prepared by:

Group 1

# 1. Introduction

This document is a Specification of all the test that we have made during our project, and in this document you can find the server test and also the client test.

# 2. Test Cases: Server chat

| Test ID | 1.1 |
| --- | --- |
| **Title** | Test login |
| **Feature** | Login inside the server chat from a client. |
| **Objective** | Test the function that manage the login. |
| **Setup** | The chat server must be turend on and use a client from a terminal. |
| **Test Data** | User information: *username* and *password*. |
| **Test Actions** | 1. Open the client and try to login. 2. Insert the correct login information and send it. 3. Wait for a response from the server.|
| **Expected Results** | The server have to send an OK message if the user information are correct, and if it is not, must send an ERROR message (see the chat protocol). |

| Test ID | 2.4 |
| --- | --- |
| **Title** | Test sending message |
| **Feature** | Send a message from a client to another. |
| **Objective** | Test the function that manage the sending of message. |
| **Setup** | The chat server must be turend on and two other client must be logged in the server. |
| **Test Data** | User information: *username*; message data: *text of the message*. |
| **Test Actions** | 1. From the client 1 select the user that you want to contact. 2. Write the text of the message. 3. Send the message. |
| **Expected Results** | The server have to recive the message from client 1, and send at the terminal an OK message, after that the server have to find the right socket associated with the recipient username, and forward it correctly. |

| Test ID | 2.5 |
| --- | --- |
| **Title** | Test sending broadcast message |
| **Feature** | Send a message from a client to all the online client. |
| **Objective** | Test the function that manage the broadcast sending of message. |
| **Setup** | The chat server must be turend on and two or more other client must be logged in the server. |
| **Test Data** | User information: *username*; message data: *text of the message*. |
| **Test Actions** | 1. From the client 1 select the broadcast mode of message. 2. Write the text of the message. 3. Send the message. |
| **Expected Results** | The server have to recive the message from client 1, and send at the terminal an OK message, after that the server have to find the socket of all the online client, and foreward the message to all of them. |

# 3. Test Cases: Client chat

**Tabella template**

| Test ID | 1.1 |
| --- | --- |
| **Title** | Login  |
| **Feature** | Login to the server from the client application |
| **Objective** | Confirm that the login protocol run correctly |
| **Setup** | The client must sent a request of login to the server and must wait an answer  |
| **Test Data** | Username and password |
| **Test Actions** | Open the client application, insert the username and password and click "login" |
| **Expected Results** | After the click on the "login" button, we must be reindered on the chat interface |

| Test ID | 1.2 |
| --- | --- |
| **Title** |  Registration with valid username and password  |
| **Feature** | Registration to the server from the client application |
| **Objective** | Confirm that the registration protocol run correctly |
| **Setup** | The client must sent a request of registration to the server and must wait an answer  |
| **Test Data** | Valid Username and password |
| **Test Actions** | Open the client application click registration, a new page must appear and insert the username and password and click "Send" |
| **Expected Results** | After the click on the "registration" button, we must be reindered on the registration page, and after the click on the "send" button we must be reindered on the chat interface |

| Test ID | 1.3 |
| --- | --- |
| **Title** |  Registration with invalid username and password  |
| **Feature** | Registration to the server from the client application |
| **Objective** | Confirm that the registration protocol run correctly |
| **Setup** | The client must sent a request of registration to the server and must wait an answer  |
| **Test Data** | Invalid Username and password |
| **Test Actions** | Open the client application click registration, a new page must appear and insert the username and password and click "Send" |
| **Expected Results** | After the click on the "registration" button, we must be reindered on the registration page, and after the click on the "send" button on the page must apper an error message |
