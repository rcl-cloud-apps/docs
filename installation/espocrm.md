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

- In the installation page, select the Azure Resource Group and the Azure App Service Plan to install the web app. The App Service Plan must be higher than the Free and Shared tiers.

- Click the 'Submit' button when you are done.

![image](../images/installation/webapp-install.png)

- **You will need to wait 15 minutes for the web app to be completely installed in the App Service Plan, so be patient.**

![image](../images/installation/operation-submitted.png)

## Installing EspoCRM

Once the web application is successfully installed in the App Service Plan, you will continue to install EspoCRM.

- Click the 'My Web Apps' menu link, and scroll down to the WordPress app

- In the 'Manage' dropdown menu, select 'Launch Web App'

![image](../images/installation/espocrm-manage.png)

- You should see the EspoCRM install page. If you do not see this page or you are presented with another page or a 'not found' message, wait for a few more minutes for the site to be installed in the App Service Plan.

- Select the language and click the 'Start' button.

![image](../images/installation/espocrm-install-lang.png)

- Accept the License Agreement

![image](../images/installation/espocrm-license.png)

- You will need to get the database connection settings from the in-app database in the App Service Plan.

- In the RCL Web Apps portal, in the web app click the 'Manage' drop down, and click on 'View web app Database Connection and Properties'

![image](../images/installation/webapp-db-conn.png)

- The database connection is shown below

![image](../images/installation/webapp-db-conn2.png)

- Enter the database settings on the EspoCRM page. The 'Host Name' should include the port (Full Host)

- Click the 'Test Connection' button 

- When you are done, click the 'Next' button

![image](../images/installation/espocrm-install-db-conn.png)

- In the 'System Requirements' section, you will notice that we need to change the following PHP.INI settings

![image](../images/installation/espocrm-settings-fail.png)

- In the RCL Web Apps portal, in the web app click the 'Manage' drop down, and click on 'View web app Database Connection and Properties'

![image](../images/installation/webapp-php-ini.png)

- In the Custom PHP.INI page, clcik the 'Create/Update custom PHP.INI' settings link

![image](../images/installation/php-ini-create.png)

- Create a text file with the following settings :

![image](../images/installation/espocrm-php-ini-file.png)

- Save the file with the file name : 'settings.ini'

- In the RCL Web App 'Create/Update Custom PHI.INI' page, select 'Non-System' Type and upload the 'settings.ini' file you created earlier. Click the Submit button when you are done

![image](../images/installation/php-ini-upload.png)

- In the RCL Web App portal, ensure that the PHI.INI settings is correctly set 

![image](../images/installation/espocrm-php-ini-settings.png)

- In the EspoCRM installation page. recheck the settings

![image](../images/installation/espocrm-php-ini-recheck.png)





