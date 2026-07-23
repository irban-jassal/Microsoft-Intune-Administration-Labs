
# Lab 1: Intune Enrollment & Device Configuration Basics

## Objective

Configure Microsoft Intune enrollment settings, create a pilot group, and deploy a Windows configuration profile for device management.

---

## Environment

- Microsoft Intune Admin Center
- Microsoft Entra ID
- Microsoft 365 Tenant

---

# Scenario

An organization is preparing Microsoft Intune to manage corporate devices. The IT administrator configures enrollment settings, creates a pilot group for testing, and applies security configurations before production deployment.

---

# Tasks Completed

## 1. Automatic Enrollment Configuration

Configured Microsoft Intune Automatic Enrollment to allow selected users to enroll devices.

### Configuration

- MDM User Scope: **Some**
- Assigned Group: **Intune-Pilot-Users**

### Purpose

MDM User Scope determines which users are allowed to automatically enroll devices into Intune.

### Screenshot

![MDM User Scope](screenshots/mdm-user-scope.png)

---

# 2. Enrollment Status Page (ESP)

Reviewed Enrollment Status Page settings used during Windows device enrollment.

### Purpose

The Enrollment Status Page helps ensure required policies and applications are applied before users access the device.

### Key Settings Reviewed

- Enrollment progress tracking
- Blocking access until setup completes
- Application and policy deployment status

### Screenshot

![Enrollment Status Page](screenshots/enrollment-status-page.png)

---

# 3. Create Intune Pilot Group

Created a security group for testing Intune policies before production deployment.

### Group Details

Group Name:


Intune-Pilot-Users


Members:

- Admin test account
- John Smith

### Purpose

Pilot groups allow administrators to test policies with a small group of users before organization-wide deployment.

### Screenshot

![Intune Pilot Group](screenshots/intune-pilot-group.png)

---

# 4. Windows Configuration Profile

Created a Windows configuration profile and assigned it to the pilot group.

### Profile Name


Windows-Device-Restrictions-Pilot


### Configured Settings

- Password required
- Minimum password length: 8 characters
- Password expiration: 30 days
- Maximum inactivity before screen lock: 15 minutes

### Assignment

Assigned to:


Intune-Pilot-Users


### Purpose

Configuration Profiles allow administrators to configure and enforce device settings after enrollment.

### Screenshot

![Configuration Profile](screenshots/configuration-profile.png)

---

# 5. Enrollment Platform Restrictions

Reviewed enrollment restrictions to control which platforms can enroll into Intune.

### Current Configuration

| Platform | Status |
|---|---|
| Windows | Allowed |
| macOS | Allowed |
| iOS/iPadOS | Allowed |
| Android | Allowed |

### Purpose

Enrollment Platform Restrictions control whether a device type is allowed to enroll into Intune.

### Screenshot

![Enrollment Platform Restrictions](screenshots/enrollment-platform-restrictions.png)

---

# 6. Device Limit Restrictions

Reviewed device enrollment limits.

### Configuration

Maximum devices per user:


5 devices


### Purpose

Device Limit Restrictions control how many devices a user can enroll into Intune.

### Screenshot

![Device Limit Restrictions](screenshots/device-limit-restrictions.png)

---

# Key Learnings

- Learned the Intune enrollment workflow.
- Understood the difference between enrollment settings and device configuration policies.
- Learned how pilot groups are used for safe policy testing.
- Learned how Configuration Profiles apply settings after enrollment.
- Understood the difference between Enrollment Restrictions and Applicability Rules.

---

# Interview Questions

## What is MDM User Scope?

MDM User Scope determines which users can automatically enroll devices into Microsoft Intune.

---

## What is the difference between Enrollment Restrictions and Configuration Profiles?

Enrollment Restrictions control whether a device can enroll into Intune.

Configuration Profiles apply settings after the device has enrolled.

---

## What is the Enrollment Status Page?

The Enrollment Status Page monitors the Windows enrollment process and ensures required policies and applications are applied before the user accesses the device.

---

## What are Configuration Profiles in Intune?

Configuration Profiles allow administrators to configure device settings such as passwords, security settings, Wi-Fi, VPN, and restrictions.


After pasting:

Click Commit changes
Open the README preview
Check that all screenshots display correctly

Then we will review it once before moving to Lab 2 – Compliance Policies. 👍

give me 1  to paste

Sure. Paste this as the full Lab 1 README:

# Lab 1: Intune Enrollment & Device Configuration Basics

## Objective

Configure Microsoft Intune enrollment settings, create a pilot group, and deploy a Windows configuration profile for device management.

---

## Environment

- Microsoft Intune Admin Center
- Microsoft Entra ID
- Microsoft 365 Tenant

---

## Scenario

An organization is preparing Microsoft Intune to manage corporate devices. The IT administrator configures enrollment settings, creates a pilot group for testing, and applies security configurations before production deployment.

---

# Tasks Completed

## 1. Automatic Enrollment Configuration

Configured Microsoft Intune Automatic Enrollment to allow selected users to enroll devices.

### Configuration

- MDM User Scope: **Some**
- Assigned Group: **Intune-Pilot-Users**

### Purpose

MDM User Scope determines which users are allowed to automatically enroll devices into Intune.

### Screenshot

![MDM User Scope](screenshots/mdm-user-scope.png)

---

## 2. Enrollment Status Page (ESP)

Reviewed Enrollment Status Page settings used during Windows device enrollment.

### Purpose

The Enrollment Status Page helps ensure required policies and applications are applied before users access the device.

### Screenshot

![Enrollment Status Page](screenshots/enrollment-status-page.png)

---

## 3. Intune Pilot Group

Created a security group for testing Intune policies before production deployment.

### Group Name


Intune-Pilot-Users


### Members

- Admin test account
- John Smith

### Purpose

Pilot groups allow administrators to test policies with a small group before deploying changes across the organization.

### Screenshot

![Intune Pilot Group](screenshots/intune-pilot-group.png)

---

## 4. Windows Configuration Profile

Created a Windows configuration profile and assigned it to the pilot group.

### Profile Name


Windows-Device-Restrictions-Pilot


### Configured Settings

- Password required
- Minimum password length: 8 characters
- Password expiration: 30 days
- Maximum inactivity before screen lock: 15 minutes

### Assignment

Assigned to:


Intune-Pilot-Users


### Purpose

Configuration Profiles allow administrators to apply and enforce device settings after enrollment.

### Screenshot

![Configuration Profile](screenshots/configuration-profile.png)

---

## 5. Enrollment Platform Restrictions

Reviewed enrollment platform restrictions to control which device platforms can enroll into Intune.

### Configuration

| Platform | Status |
|---|---|
| Windows | Allowed |
| macOS | Allowed |
| iOS/iPadOS | Allowed |
| Android | Allowed |

### Purpose

Enrollment Platform Restrictions determine which device platforms are allowed or blocked from enrolling into Intune.

### Screenshot

![Enrollment Platform Restrictions](screenshots/enrollment-platform-restrictions.png)

---

## 6. Device Limit Restrictions

Reviewed device enrollment limits.

### Configuration

Maximum devices per user:


5 devices


### Purpose

Device Limit Restrictions control how many devices a single user can enroll into Intune.

### Screenshot

![Device Limit Restrictions](screenshots/device-limit-restrictions.png)

---

# Key Learnings

- Learned the Microsoft Intune enrollment workflow.
- Understood the difference between enrollment settings and configuration profiles.
- Learned how pilot groups are used for testing policies.
- Learned how configuration profiles apply settings after device enrollment.
- Understood the difference between Enrollment Restrictions and Applicability Rules.

---
