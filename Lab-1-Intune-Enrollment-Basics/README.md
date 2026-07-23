
# Lab 1: Intune Enrollment & Device Configuration Basics

## Objective

Configure Microsoft Intune enrollment settings and create a Windows configuration profile for device management.

---

## Environment

- Microsoft Intune Admin Center
- Microsoft Entra ID
- Microsoft 365 Tenant

---

## Scenario

An organization is preparing Microsoft Intune to manage corporate devices. The administrator configures enrollment settings and deploys device configuration policies for testing before production rollout.

---

# Tasks Completed

## 1. Automatic Enrollment Configuration

Configured Microsoft Intune Automatic Enrollment settings.

### Configuration

- MDM User Scope: **Some**
- Assigned Group: **Intune-Pilot-Users**

### Purpose

MDM User Scope controls which users are allowed to automatically enroll devices into Intune.

### Screenshot

![Automatic Enrollment](screenshots/automatic-enrollment.png)

---

## 2. Enrollment Status Page (ESP)

Reviewed Enrollment Status Page settings used during Windows device enrollment.

### Purpose

The Enrollment Status Page provides visibility during device setup and helps ensure required policies and applications are applied before users access the device.

### Screenshot

![Enrollment Status Page](screenshots/enrollment-status-page.png)

---

## 3. Windows Configuration Profile

Created a Windows configuration profile and assigned it to the pilot group.

### Profile Name


Windows-Device-Restrictions-Pilot


### Configured Settings

- Password required
- Minimum password length: 8 characters
- Password expiration: 30 days
- Maximum inactivity before screen lock: 15 minutes

### Purpose

Configuration Profiles allow administrators to apply and enforce device settings after enrollment.

### Screenshot

![Configuration Profile](screenshots/configuration-profile.png)

---

## 4. Enrollment Platform Restrictions

Reviewed enrollment platform restrictions.

### Configuration

| Platform | Status |
|---|---|
| Windows | Allowed |
| macOS | Allowed |
| iOS/iPadOS | Allowed |
| Android | Allowed |

### Purpose

Enrollment Platform Restrictions control which device platforms are allowed to enroll into Intune.

### Screenshot

![Enrollment Platform Restrictions](screenshots/enrollment-platform-restrictions.png)

---

# Key Learnings

- Learned the Intune enrollment workflow.
- Understood the difference between enrollment settings and configuration profiles.
- Learned how configuration profiles apply settings after enrollment.
- Understood the difference between Enrollment Restrictions and Applicability Rules.

---

# Interview Questions

## What is MDM User Scope?

MDM User Scope determines which users can automatically enroll devices into Intune.

## What is the difference between Enrollment Restrictions and Configuration Profiles?

Enrollment Restrictions control whether a device can enroll into Intune.

Configuration Profiles apply settings after the device is enrolled.

## What is Enrollment Status Page?

ESP monitors the Windows enrollment process and ensures required policies and applications are a
