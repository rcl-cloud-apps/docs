---
title: phpList
description: Learn how to install phpList in an Azure App Service Plan using RCL Web Apps
parent: Installation
nav_order: 4
---

# Introduction

In this section, you will learn how to install phpList in a Azure App Service Plan using RCL Web Apps.

# Requirements

An **Azure App Service Plan** is required for this installation. The App Service Plan must be :

- Higher than the Free and Shared Tier
- A Windows Server

# Installation

## App Service Plan

- In the RCL Web Apps portal, click on the 'Install Web Apps' menu item

- Then click the 'Install' button in the phpList panel

![image](../images/installation/phplist-install.png)

- In the installation page, select the Azure Resource Group and the Azure App Service Plan to install the web app. The App Service Plan must be higher than the Free and Shared tiers.

- Click the 'Submit' button when you are done.

![image](../images/installation/webapp-install.png)

- **You will need to wait 15 minutes for the web app to be completely installed in the App Service Plan, so be patient.**

![image](../images/installation/operation-submitted.png)

## Installing phpList

Once the web application is successfully installed in the App Service Plan, you will continue to install phpList.

### Setting Up The Database

- You will need to get the database connection settings from the in-app database in the App Service Plan

- In the RCL Web Apps portal, in the phpList web app click the 'Manage' drop down, and click on 'View web app Database Connection and Properties'

![image](../images/installation/webapp-db-conn.png)

- The database connection is shown below

![image](../images/installation/webapp-db-conn2.png)

- In the 'Manage' drop down, lick on 'Use Kudu to configure web app files'

- In Kudu, click on 'CMD' in the 'Debug console' menu link

- Navigate to site/wwwroot/lists/config

![image](../images/installation/phplist-kudu-config.png)

- Edit the config.php file to configure the database connection

![image](../images/installation/phplist-kudu-config-db.png)

## Setting Up SMTP Email Sender

- Configure an external mail server for handling phpList email

- The following example shows the settings in the config.php file for sending emails from a gmail account

![image](../images/installation/phplist-smtp-configure.png)

## Initializing The Database

- In the RCL Web Apps portal, in the phpList web app click the 'Manage' drop down, and click on 'Launch Web App'

- In the phpList install page, click on the 'Initialise Database' link

![image](../images/installation/phplist-db-initialize.png)

- Add the information to initialize the database and click the 'Continue' button when you are done

![image](../images/installation/phplist-db-initialize-info.png)

- Ensure the database is successfully initialized

![image](../images/installation/phplist-db-initialize-done.png)


## Configuring Gmail 

If you are using Gmail to send emails, you will need to [allow less secure apps](https://support.google.com/accounts/answer/6010255?hl=en) in your Google account.

![image](../images/installation/phplist-google-security-app.png)

You may need to also resolve Gmail security issues by clicking 'Yest, it was me'

![image](../images/installation/phplist-google-security-alert.png)

## Start Using the Application

- Login to the admin Portal and start using the application

![image](../images/installation/phplist-admin-portal.png)
