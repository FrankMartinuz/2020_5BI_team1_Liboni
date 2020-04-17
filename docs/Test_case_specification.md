Roo Balance Test Case Specification

# Test Case Specification

# For

# Team 1

December 7, 2010

Prepared by:

Casey Droneburg

# **Table of Contents**

**1 Introduction 4**

**2 Test Cases: iOS Application 4**

**3 Test Cases: Proxy Server 6**

Revision History

| **Version** | **Date** | **Name** | **Description** |
| --- | --- | --- | --- |
| 1 | 11/11/10 | Casey Droneburg | Initial Document |
| 2 | 12/07/10 | Casey Droneburg | Updated test case numbers to eliminate typographical errors; added test case 3.2 (proxy server: incorrect password) which was left out |

# 1Introduction

This document provides the test cases to be carried out for the Roo Balance Application. Each item to be tested is represented by an individual test case. Each case details the input and expected outputs.

# 2Test Cases: iOS Application

| Test ID | 2.1 |
| --- | --- |
| Title | Correct Login |
| Feature | Login to umkc.manageMyID.com with Roo Balance App |
| Objective | Confirm that proper user id an password yields access to the website as expected. |
| Setup | IOS device or simulator has Roo Balance application ready to run. |
| Test Data | Login informationUser Email = [cdbpc@umkc.edu](mailto:cdbpc@umkc.edu)Password = r00bucks |
| Test Actions | 1. Start Roo Balance application2. Select View Account option3. Enter login information |
| Expected Results | System displays account balance with option to logoff. Account balance should match that found on umkc.ManageMyID.com. |

| Test ID | 2.2 |
| --- | --- |
| Title | Incorrect Password |
| Feature | Login to umkc.manageMyID.com with Roo Balance App |
| Objective | Confirm that valid user id with an invalid password denies access to the website without leaving the user stranded. |
| Setup | IOS device or simulator has Roo Balance application ready to run. |
| Test Data | Correct user e-mail, incorrect passwordUser Email = [cdbpc@umkc.edu](mailto:cdbpc@umkc.edu)Password = password |
| Test Actions | 1. Start Roo Balance application2. Select View Account option3. Enter invalid login information |
| Expected Results | System displays error message with option to try again. |

| Test ID | 2.3 |
| --- | --- |
| Title | Incorrect User E-Mail |
| Feature | Login to umkc.manageMyID.com with Roo Balance App |
| Objective | Confirm that invalid user id denies access to the website without leaving the user stranded. |
| Setup | IOS device or simulator has Roo Balance application ready to run. |
| Test Data | Incorrect user e-mail, incorrect passwordUser Email = [l](mailto:cdbpc@umkc.edu)ogin@umkc.eduPassword = password |
| Test Actions | 1. Start Roo Balance application2. Select View Account option3. Enter invalid login information |
| Expected Results | System displays error message with option to try again. |

| Test ID | 2.4 |
| --- | --- |
| Title | Select Option View Locations |
| Feature | Display merchant locations accepting Roo Bucks. |
| Objective | Confirm that a list of locations is displayed after the user selects the option. |
| Setup | IOS device or simulator has Roo Balance application ready to run. |
| Test Data |
 |
| Test Actions | 1. Start Roo Balance application2. Select View Locations option |
| Expected Results | System displays list of merchants with addresses. |

| Test ID | 2.5 |
| --- | --- |
| Title | Select Option View Transactions |
| Feature | Display recent Roo Bucks account transactions. |
| Objective | Confirm that recent transactions are displayed properly. |
| Setup | IOS device or simulator has Roo Balance application ready to run. |
| Test Data | Login informationUser Email = [cdbpc@umkc.edu](mailto:cdbpc@umkc.edu)Password = r00bucks |
| Test Actions | 1. Start Roo Balance application2. Select View Account option3. Select View Transactions option |
| Expected Results | System displays recent transactions legibly with option to logoff. Recent transactions should match that found on umkc.ManageMyID.com. |

# 3Test Cases: Proxy Server

| Test ID | 3.1 |
| --- | --- |
| Title | Correct Login |
| Feature | Login to umkc.manageMyID.com via proxy server |
| Objective | Confirm that proper user id an password yields access to the website as expected. |
| Setup | Access to internet: [http://206.123.75.42:7070/post.html](http://206.123.75.42:7070/post.html)[https://206.123.75.42:7071/post.html](https://206.123.75.42:7071/post.html) |
| Test Data | Login informationUser Email = [cdbpc@umkc.edu](mailto:cdbpc@umkc.edu)Password = r00bucks |
| Test Actions | 1. Go to proxy server http site defined in setup.2. Enter correct login information3. Press submit |
| Expected Results | Site displays numeric balance for account. Numeric balance matches that from umkc.ManageMyID.com. |

| Test ID | 3.2 |
| --- | --- |
| Title | Incorrect Password |
| Feature | Login to umkc.manageMyID.com via proxy server |
| Objective | Confirm that invalid password denies access to the website and returns an error. |
| Setup | Access to internet: [http://206.123.75.42:7070/post.html](http://206.123.75.42:7070/post.html)[https://206.123.75.42:7071/post.html](https://206.123.75.42:7071/post.html) |
| Test Data | Login informationUser Email = cdbpc@umkc.eduPassword = password |
| Test Actions | 1. Go to proxy server http site defined in setup.2. Enter login information as defined in test data3. Press submit4. View page source. |
| Expected Results | Error tag is evident in page source. |

| Test ID | 3.3 |
| --- | --- |
| Title | Incorrect User E-Mail Login |
| Feature | Login to umkc.manageMyID.com via proxy server |
| Objective | Confirm that invalid user id denies access to the website and returns an error. |
| Setup | Access to internet: [http://206.123.75.42:7070/post.html](http://206.123.75.42:7070/post.html)[https://206.123.75.42:7071/post.html](https://206.123.75.42:7071/post.html) |
| Test Data | Login informationUser Email = login@umkc.eduPassword = password |
| Test Actions | 1. Go to proxy server http site defined in setup.2. Enter login information as defined in test data3. Press submit4. View page source. |
| Expected Results | Error tag is evident in page source. |

| Test ID | 3.4 |
| --- | --- |
| Title | View Transactions via Proxy Server |
| Feature | View transaction history on umkc.manageMyID.com via proxy server |
| Objective | Confirm that transaction history is accessed and retrieved from the website correctly. |
| Setup | Access to internet: [http://206.123.75.42:7070/post.html](http://206.123.75.42:7070/post.html)[https://206.123.75.42:7071/post.html](https://206.123.75.42:7071/post.html) |
| Test Data | Login informationUser Email = [cdbpc@umkc.edu](mailto:cdbpc@umkc.edu)Password = r00bucks |
| Test Actions | 1. Go to proxy server http site defined in setup.2. Enter login information as defined in test data3. Press submit4. View page source. |
| Expected Results | Recent transactions are displayed and numbers match those on umkC.ManageMyID.com. |

Last Modified: 12/07/2010 Page 8 of 8
