---
title: EspoCRM
description: Learn how to install EspoCRM in an Azure App Service Plan using RCL Web Apps
parent: Installation
nav_order: 2
---

# Introduction

In this section, you will learn how to install EspoCRM in as Azure App Service Plan using RCL Web Apps.

# Requirements

An **Azure App Service Plan** is required for this installation. The App Service Plan must be :

- Higher than the Free and Shared Tier
- A Windows Server

# Installation

## App Service Plan

- In the RCL Web Apps portal, click on the 'Install Web Apps' menu item

- Then click the 'Install' button in the EspoCRM panel

![image](../images/installation/espocrm-install.png)

- In the installation page, select the Azure Resource Group and the Azure App Service Plan to install the web app. The App Service Plan must be higher than the Free and Shared tiers

- Click the 'Submit' button when you are done

![image](../images/installation/webapp-install.png)

- **You will need to wait 15 minutes for the web app to be completely installed in the App Service Plan, so be patient.**

![image](../images/installation/operation-submitted.png)

## Installing EspoCRM

Once the web application is successfully installed in the App Service Plan, you will continue to install EspoCRM.

- Click the 'My Web Apps' menu link, and scroll down to the EspoCRM app

- In the 'Manage' dropdown menu, select 'Launch Web App'

![image](../images/installation/espocrm-manage.png)

- You should see the EspoCRM install page. If you do not see this page, wait for a few more minutes for the site to be installed in the App Service Plan.

![image](../images/installation/espocrm-install-lang.png)

## Custom PHP.INI Settings 

EspoCRM requires custom PHP.INI settings. Follow these instructions to create the settings :

- In the RCL Web Apps portal, click on the 'Manage' button for the EspoCRM web app

- Click on the 'Custom PHP.INI settings' link

![image](../images/installation/espocrm-manage.png)

- In the 'Custom PHP.INI Settings' page, click on the 'Create/Update custom PHP.INI settings' link

![image](../images/installation/php-ini-create.png)

- Create a text file with the following settings :

![image](../images/installation/espocrm-php-ini-file.png)

- Save the file with the file name : 'settings.ini'

- In the RCL Web App 'Create/Update Custom PHI.INI' page, select 'Non-System' Type and upload the 'settings.ini' file you created earlier. Click the Submit button when you are done

![image](../images/installation/php-ini-upload.png)

- In the RCL Web App portal, ensure that the PHI.INI settings is correctly set for EspoCRM

- You will need to restart the app for the settings to take effect

![image](../images/installation/espocrm-php-ini-settings.png)

- In the RCL Web Apps portal, click the 'Restart' button for the EspoCRM web app. Wait for few minutes for the app to restart before you continue with the installation.

![image](../images/installation/espocrm-manage.png)

## Setting Up The Database

- Open the EspoCRM app and continue the installation

- Select the language and click the 'Start' button

![image](../images/installation/espocrm-install-lang.png)

- Accept the License Agreement

![image](../images/installation/espocrm-license.png)

- You will need to get the database connection settings from the in-app database in the App Service Plan.

- In the RCL Web Apps portal, in the EspoCRM web app click the 'Manage' drop down, and click on 'View web app Database Connection and Properties'

![image](../images/installation/webapp-db-conn.png)

- The database connection is shown below

![image](../images/installation/webapp-db-conn2.png)

- Enter the database settings on the EspoCRM page. The 'Host Name' should include the port (Full Host)

- Click the 'Test Connection' button 

- When you are done, click the 'Next' button

![image](../images/installation/espocrm-install-db-conn.png)

- Ensure the system requirements (including the custom setting we created earlier) passes the validation tests. Click the 'Next' button to proceed

![image](../images/installation/espocrm-system-requirements.png)

- Set the Username and Password to login and click the 'Next' button

![image](../images/installation/espocrm-set-password.png)

- Set the 'System Settings' and complete the installation

![image](../images/installation/espocrm-system-settings.png)

- Login to the admin portal to start using the app

![image](../images/installation/espocrm-admin-portal.png)

## Cron Job

You must verify that the EspoCRM cron jobs are running successfully.

- In the RCL Web Apps portal, in the EspoCRM web app click the 'Manage' drop down, and click on 'Setup Cron jobs' link

![image](../images/installation/espocrm-manage.png)

- In the 'Cron Jobs' page, click the 'View Cron (web) Jobs Dashboard

![image](../images/installation/espocrm-cron-job.png)

- Ensure the cron jobs are successfully running every 5 minutes

![image](../images/installation/espocrm-cron-job-dashboard.png)








