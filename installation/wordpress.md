---
title: WordPress
description: Learn how to install WordPress in an Azure App Service Plan using RCL Web Apps
parent: Installation
nav_order: 1
---

# Introduction

In this section, you will learn how to install WordPress in a Azure App Service Plan using RCL Web Apps.

# Requirements

An **Azure App Service Plan** is required for this installation. The App Service Plan must be :

- Higher than the Free and Shared Tier
- A Windows Server

# Installation

## App Service Plan

- In the RCL Web Apps portal, click on the 'Install Web Apps' menu item

- Then click the 'Install' button in the WordPress panel

![image](../images/installation/wordpress-install.png)

- In the installation page, select the Azure Resource Group and the Azure App Service Plan to install the web app. The App Service Plan must be higher than the Free and Shared tiers.

- Click the 'Submit' button when you are done.

![image](../images/installation/webapp-install.png)

- **You will need to wait 15 minutes for the web app to be completely installed in the App Service Plan, so be patient.**

![image](../images/installation/operation-submitted.png)

## Installing WordPress

Once the web application is successfully installed in the App Service Plan, you will continue to install WordPress.

- Click the 'My Web Apps' menu link, and scroll down to the WordPress app

- In the 'Manage' dropdown menu, select 'Launch Web App'

![image](../images/installation/wordpress-manage.png)

- You should see the WordPress install page. If you do not see this page or you are presented with another page or a 'not found' message, wait for a few more minutes for the site to be installed in the App Service Plan.

- Select the language and click the 'Continue' button.

![image](../images/installation/wordpress-install-lang.png)

- Provide the information needed for the installation and click the 'Install WordPress' button

![image](../images/installation/wordpress-install-info.png)

- Wait for a few minutes for the installation to complete. Then, click the 'Log In' button to login to the WordPress Admin Portal.

![image](../images/installation/wordpress-install-login.png)

- Enter the UserName and Password that you previously set and click the 'Login' button.

![image](../images/installation/wordpress-install-login2.png)

- You can start building your website in the WordPress Admin Portal.

![image](../images/installation/wordpress-admin-portal.png)




