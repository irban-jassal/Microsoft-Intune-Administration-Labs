 Lab 08 - Microsoft Store App (new) Deployment using Microsoft Intune

## Overview

In this lab, I deployed a Microsoft Store application using Microsoft Intune.

This lab demonstrates how administrators can deploy applications from the Microsoft Store to managed Windows devices without packaging a Win32 application.

---

## Lab Objectives

- Create a Microsoft Store application in Intune
- Configure application information
- Review application settings
- Assign the application to a user group
- Review and create the deployment

---

## Lab Environment

| Component | Value |
|----------|-------|
| Platform | Microsoft Intune Admin Center |
| Identity | Microsoft Entra ID |
| App Type | Microsoft Store app (new) |
| Assignment Group | Intune-Pilot-Users |

---

# Configuration Steps

## Step 1 - Select App Type

Navigation:


Microsoft Intune Admin Center
→ Apps
→ All Apps
→ Add


Selected:


Microsoft Store app (new)


### Screenshot

![Select App Type](Lab8_Select_App_Type.png)

---

## Step 2 - Configure Application Information

Configured the application details including:

- Application Name
- Publisher
- Description
- Version
- Application Logo

### Screenshot

![Application Information](Lab8_App_Information.png)

---

## Step 3 - Review Application Overview

Verified the application configuration before proceeding with deployment.

### Screenshot

![Application Overview](Lab8_App_Overview.png)

---

## Step 4 - Assign the Application

Assigned the application to the following group:


Intune-Pilot-Users


Assignment Type:


Required


### Screenshot

![Application Assignment](Lab8_App_Assignment.png)

---

## Step 5 - Review and Create

Reviewed all configuration settings and created the application deployment.

### Screenshot

![Review and Create](Lab8_Review_Create.png)

---

# Skills Demonstrated

- Microsoft Intune Application Management
- Microsoft Store App Deployment
- Application Assignment
- Microsoft Entra ID Group Assignment
- Endpoint Management

---

# Key Takeaways

This lab provided hands-on experience deploying Microsoft Store applications using Microsoft Intune.

Using Microsoft Store apps allows administrators to deploy supported applications directly from Microsoft Intune without creating Win32 packages.

---

# Lab Status

Completed

