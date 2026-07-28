
# Lab 6 – Windows Enrollment Restrictions in Microsoft Intune

## Objective

The objective of this lab was to configure Windows enrollment restrictions in Microsoft Intune to control which devices can enroll into Intune and manage device ownership settings.

The lab demonstrates how administrators control device enrollment before devices become managed endpoints.

---

# Environment

- Microsoft Intune Admin Center
- Microsoft Entra ID
- Microsoft 365 Tenant
- Assignment Group: Intune-Pilot-Users

---

# Scenario

An organization is preparing Microsoft Intune for endpoint management.

Before allowing devices to enroll, administrators need to define enrollment restrictions to control:

- Allowed device platforms
- Device ownership restrictions
- Personal device enrollment
- Enrollment access policies

---

# Tasks Completed

## 1. Windows Enrollment Restriction Configuration

Configured Windows enrollment restrictions to allow Windows devices to enroll into Microsoft Intune.

### Configuration

Platform:

Windows

MDM:

Allow

---

## 2. Personally Owned Device Enrollment

Configured personal device enrollment settings.

### Configuration

Personally Owned Devices:

Allow

### Purpose

This setting controls whether users can enroll personally owned Windows devices into Intune.

In production environments, organizations may block personal devices depending on security requirements and BYOD policies.

---

## 3. Device Enrollment Assignment

Assigned the enrollment restriction policy to:

Intune-Pilot-Users


### Purpose

Pilot groups allow administrators to test enrollment policies with a controlled group before organization-wide deployment.

---

# Screenshots

## Enrollment Restriction Settings

Lab6_Windows_Enrollment_1.png

Shows:

- MDM enrollment setting
- Personally owned device configuration


## Assignment Configuration

Lab6_Windows_Enrollment_2.png

Shows:

- Policy assignment
- Intune-Pilot-Users group


## Review and Create

Lab6_Windows_Enrollment_3.png

Shows:

- Final policy review before creation

---

# Key Learnings

Through this lab, I learned:

- How Intune enrollment restrictions control device onboarding
- The difference between enrollment controls and compliance policies
- How personal device enrollment is managed
- How pilot groups are used for controlled deployment
- How organizations restrict device enrollment before applying management policies

---

# Skills Demonstrated

- Microsoft Intune Administration
- Endpoint Management
- Device Enrollment Management
- Microsoft Entra ID Integration
- Enterprise Device Governance
