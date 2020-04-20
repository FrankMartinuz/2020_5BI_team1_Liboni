Client Chat System Documentation

# System Documentation

**Team 1**

April 20, 2020

**Team Members**

Riccardo Radosta

Matteo Tognella

## Contents

1. Introduction

2. Install Python

3. Install client chat application

4. Install on Simulator or Device

5. System Maintenance

## Revision History

| Version | Date | Name | Description |
| :---: | --- | --- | --- |
| 1 | 20/04/2020 | Riccardo Radosta, Matteo Tognella | Initial Document |

## 1. Introduction

The chat client is a software that allows you to connect to a server that are using the chat protocol made by prof. De Carli.  
This protocol allows you to chat with other client chat that are using the same protocol.  
This document will explain you how to setup your device to use this sofware.

## 2. Setup the client chat software

  1. Before begin using this software ou will need to install the last version of python, and you can download it from this [link](https://www.python.org/downloads/).
  2. After you have download it, you need to open and install it, by following the instructions in the installer file.
  3. Now you need to check the installation, and to do that, you can use this command: python --version.

## 3. Install client chat application

  1. Now you have all of what you need, and we can proceed in the installation.
  2. First of all you need to download the source file of the client software, from this [link](https://github.com/FrankMartinuz/2020_5BI_team1_Liboni/tree/master/bin/ClientChat/bin)
  3. Now put all of that file inside a folder and place it where you want to place the programm, but pay attention to not change to file ordere inside the folder.
  4. Open the Graphic_client.py with python and you have done the installation.

## 4. Install on Simulator or Device

### 4.1 Required Components

Access to a computer with the iOS SDK is required in order to use Xcode and the simulator.

An iOS-compatible device is required to run application outside of the simulator. Examples include the iPhone, iPod Touch, and iPad.

### 4.2 Install Code

1. Launch Xcode
2. Configure SCM to access the code in the repository.
  1. Click on SCM → Configure SCM
  2. Click &#39;+&#39; to add new repository
  3. Name the repository RooBucks
  4. Enter URL of repository given in section 3
  5. Apply changes
3. Load code for the project
  1. Click SCM-\&gt; Repository
  2. Select RooBucks and Checkout
4. Open project &quot;RooBucks.xcodeproj&quot; from checked-out directory in Xcode.
5. Ensure that the drop-down menu in the top-left corner of the project
 window is set to the &quot;Simulator&quot; target OR that a suitable device and
 provisioning data are present.
6. Choose Build --\&gt; Build and Go in Xcode.
7. App is now running and usable.

## 5 System Maintenance

### 5.1 Objective-C Code

The user interface consists of four tabs for viewing information, plus the login screen. Each of these is implemented in one XIB file and one controller class. There are two additional XIB files: the application root view (&quot;MainView.xib&quot;) and tab bar navigation view (&quot;RooBucksTabs.xib&quot;).

On the first run, the application displays the login screen. Once the user has logged in, the view is switched to the tab bar, which is displayed at the bottom of the screen. The tab bar view enables the user to navigate between the tabs mentioned above, and hosts the four subviews for each type of information.

The logic in each view controller class mainly performs the task of pulling the appropriate data from XMLParser, formatting it, and displaying it in the correct fields. The login controller class also contains logic to store the user&#39;s credentials in the system Keychain.

### 5.2 Perl Proxy Code

The proxy server consists of a perl cgi, executed by apache when a specific POST is received via https. The perl code logs into managemyid using the user&#39;s credentials (provided in POST). From there, the code captures an https re-direct, and uses the unique URL in the re-direct to request account balance and account history. This is accomplished in three separate https transactions with managemyid.

As information is gleaned from the second two tranactions with managemyid, the perl script generates XML, and sends it to the objective-C parser on the iOS device through the (still open) tcp stream.

When the parsing and XML generation is complete, the tcp session is closed, and the perl script exits. No passwords or user data is retained on the proxy server.
