# **Server User Guide**

**Team 1 - Server**

April 17, 2020

**Team Members**

Andrea Liboni

Francesco Martino

# Contents

1. Introduction

2. Quick Start Guide

3. System Requirements

4. Main Scenarios of Use

5. Troubleshooting

## 1. Introduction

  The server chat software allow users to send text message between all type of clients(in the same network) that are using the chat protocol made by prof. De Carli.  
  In this document there are not so much things to say, because the client does not have an user interface like the client, but have only a command line output.

## 2. Quick Start Guide

1. Make sure that you have installed Python on your server/PC.

2. Set the right IP address for you server, by opening the main.py with an text editor, and modify the 273 line of the file.

3. Open the main.py file and launch the server.

## 3. System Requirements

To run the server software you will need the last Python version installed in your server/PC.

## 4. Main Scenarios of Use

  **4.1. View the user connected**

  1. Open the main.py file.
  2. Wait for the startup of the server.
  3. By now when a user connect to your server you will see him IP address and name.

  **4.2 View user credentials**

  1. In the root folder of the server software.
  2. Open the User folder.
  3. Open the user.csv file with an text editor (or Excel).

## 5. Troubleshooting

  **5.1 Network error**
  - Make sure that the IP address that you are using is valid inside your network.
  - Make sure that the application port that you are using is not used by other application.
  - Reboot the server software.
  - Reboot the server/PC.
  - Reboot your router.

  **5.2 Client unreachable**
  - Make sure that the client is inside your network.
  - Check the firewall of the client, it can block some packet.
  - Make sure that the client si using the same protocol as the server.
  - Reboot the client.
  - Reboot the server/PC.
  - Reboot your router.
