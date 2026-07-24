# Lab 2: Microsoft Intune Compliance Policies & Conditional Access

## Objective

Create a Windows compliance policy in Microsoft Intune, configure security requirements, assign the policy to a pilot group, and integrate it with Microsoft Entra Conditional Access to understand how device compliance controls access to organizational resources.

---

## Environment

- Microsoft Intune Admin Center
- Microsoft Entra Admin Center
- Microsoft 365 Developer Tenant

---

## Scenario

An organization wants to ensure that only secure and compliant Windows devices can access Microsoft 365 resources. As the Intune administrator, I created a compliance policy, configured security requirements, assigned it to a pilot group, and integrated it with a Conditional Access policy.

---

# Tasks Completed

## 1. Created Windows Compliance Policy

Created a Windows 10/11 Compliance Policy.

### Configuration

- Platform: Windows 10 and later
- Profile Type: Windows 10/11 Compliance Policy

### Purpose

Compliance Policies evaluate whether devices meet an organization's security requirements. They do not configure devices; they verify compliance.

### Screenshots

![Compliance Policy Properties](screenshots/compliance-policy-proprties1.png)

![Compliance Policy Configuration](screenshots/compliance-policy-properties2.png)

---

# 2. Configured Device Health

Configured device health requirements including:

- Require BitLocker
- Require Secure Boot
- Require Code Integrity

### Purpose

These settings help verify that Windows devices meet baseline security standards before being considered compliant.

---

# 3. Configured System Security

Configured the following security requirements:

### Password

- Require password
- Block simple passwords
- Password type: Alphanumeric
- Minimum password length: 8
- Password expiration: 30 days
- Password required after 15 minutes of inactivity
- Prevent reuse of previous 5 passwords

### Device Security

- Require encryption
- Require Firewall
- Require TPM
- Require Antivirus
- Require Antispyware

### Microsoft Defender

- Require Microsoft Defender Antivirus
- Require Security Intelligence to be up to date
- Require Real-Time Protection

### Purpose

These settings ensure enrolled Windows devices comply with the organization's security baseline before being granted access.

---

# 4. Assigned Policy

Assigned the compliance policy to:

```
Intune-Pilot-Users
```

### Purpose

Pilot groups allow administrators to validate policies with a small group before deploying them organization-wide.

---

# 5. Reviewed Compliance Reports

Reviewed the compliance reporting section after policy deployment.

### Result

No devices were available for evaluation because no Windows devices were enrolled in Microsoft Intune during this lab.

### Screenshot

![Compliance Report](screenshots/compliance-report-no-devices.png)

---

# 6. Integrated Compliance Policy with Conditional Access

Created a Conditional Access policy requiring compliant devices before accessing organizational resources.

### Policy Name

```
Require-Compliant-Device-Access
```

### Configuration

- Assigned to Intune-Pilot-Users
- Target Resources: All resources
- Grant Access
- Require device to be marked as compliant
- Policy State: Report-only

### Purpose

Conditional Access uses the compliance status reported by Intune to determine whether users are allowed to access Microsoft 365 resources.

### Screenshots

![Conditional Access Overview](screenshots/conditional-access-policy-overview.png)

![Grant Control](screenshots/conditional-access-grant-control.png)

---

# Production Considerations

During this lab, the Conditional Access policy was configured in **Report-only** mode because Microsoft Security Defaults were enabled.

In a production environment, administrators should:

- Disable Security Defaults before enforcing Conditional Access policies.
- Test policies using Report-only mode.
- Deploy policies to pilot users first.
- Validate results before enabling enforcement for all users.

---

# Key Learnings

- Learned how Compliance Policies evaluate device security.
- Configured Device Health and System Security requirements.
- Understood the difference between Configuration Profiles and Compliance Policies.
- Learned how Intune reports compliance status to Microsoft Entra ID.
- Integrated Intune Compliance with Conditional Access.
- Learned why Security Defaults must be disabled before enforcing Conditional Access policies in production.
- Understood the importance of pilot groups and Report-only mode during policy deployment.

---
