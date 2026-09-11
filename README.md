# Microsoft 365 Administration Lab

## Overview

This lab demonstrates hands-on administration of a Microsoft 365 business environment.

The objective was to simulate common tasks performed by an **IT Support Technician, Help Desk Technician, Microsoft 365 Administrator, or Junior System Administrator**.

The lab covered the complete user lifecycle, including:

- User creation and licensing
- Exchange Online administration
- Email aliases
- Shared mailboxes
- Distribution lists
- Automatic replies
- Mail forwarding
- Microsoft Teams administration
- SharePoint Online
- OneDrive
- Password resets
- Sign-in management
- Microsoft 365 Service Health
- Employee offboarding

---

## Lab Environment

**Platform:** Microsoft 365 Business Premium  
**Administration Portals:**

- Microsoft 365 Admin Center
- Exchange Admin Center
- Teams Admin Center
- SharePoint Admin Center
- Microsoft Outlook
- Microsoft OneDrive

### Test Accounts

Two types of accounts were used:

**Administrator Account**
- Used to manage Microsoft 365 services
- Managed users, licenses, mailboxes, Teams, SharePoint, and permissions

**Employee Account**
- Test employee: John Wrick
- Job Title: Support Coordinator
- Department: Operations
- Used to simulate a normal company employee

---

# Phase 1 – User Creation and Licensing

The first task was to create a new employee account using the Microsoft 365 Admin Center.

The employee was created as a normal user without administrative privileges.

### Tasks Completed

- Created a new Microsoft 365 user
- Configured employee profile information
- Assigned Microsoft 365 Business Premium
- Verified the employee appeared under Active Users
- Tested the employee's first sign-in
- Verified Outlook access

### Active Users

![Active Users](Lab%20Microsoft365%20Administration/01-Active-Users.png)

### Employee Profile

![John Profile](Lab%20Microsoft365%20Administration/02-John-Profile.png)

### Microsoft 365 License

Microsoft 365 Business Premium was assigned to the employee.

This provided access to Microsoft 365 services such as:

- Exchange Online
- Outlook
- Teams
- SharePoint
- OneDrive
- Microsoft 365 applications

![John License](Lab%20Microsoft365%20Administration/03-John-License.png)

---

# Phase 2 – Exchange Online Administration

Exchange Online was used to manage the employee's corporate mailbox.

The employee's mailbox was verified through the Exchange Admin Center.

### Mailbox Administration

![John Mailbox](Lab%20Microsoft365%20Administration/04-John-Mailbox.png)

---

## Email Alias

An additional email address was added to John's mailbox.

An email alias allows multiple email addresses to deliver messages to the same mailbox without creating another user account.

Example:

```text
Primary email → Employee mailbox
Alias → Same employee mailbox
```

The alias was tested by sending an email to the additional address and confirming that it arrived in John's normal Outlook inbox.

![Email Alias](Lab%20Microsoft365%20Administration/05-Email-Alias.png)

---

# Phase 3 – Shared Mailbox

A shared mailbox named **IT Support** was created.

Shared mailboxes are commonly used for departmental addresses such as:

```text
support@company.com
helpdesk@company.com
hr@company.com
sales@company.com
```

Unlike a normal mailbox, a shared mailbox can be accessed by multiple authorized employees.

### IT Support Shared Mailbox

![Shared Mailbox](Lab%20Microsoft365%20Administration/06-Shared-Mailbox.png)

### Mailbox Permissions

John was granted permissions to use the shared mailbox.

The permissions included:

**Read and Manage**

Allows the user to open and manage the shared mailbox.

**Send As**

Allows the user to send email directly as the shared mailbox.

**Send on Behalf**

Allows the user to send a message on behalf of the shared mailbox.

![Shared Mailbox Permissions](Lab%20Microsoft365%20Administration/07-Shared-Mailbox-Permissions.png)

The configuration was tested through Outlook to confirm that the employee could access the IT Support mailbox and send messages using the shared mailbox address.

---

# Phase 4 – Distribution List

A distribution list named **IT TEAM** was created.

A distribution list provides one email address that distributes a message to multiple users.

Example:

```text
Email sent to IT TEAM
        |
        +----> Administrator
        |
        +----> John Wrick
```

This is different from a shared mailbox.

**Shared Mailbox**

Multiple users work from the same mailbox.

**Distribution List**

A copy of the email is delivered to each member's individual mailbox.

![Distribution List](Lab%20Microsoft365%20Administration/08-Distribution-List.png)

The distribution list was tested by sending an email to the group address and confirming delivery to the members.

---

# Phase 5 – Automatic Replies

Automatic replies were configured for the employee.

This simulates a common scenario where an employee is:

- On vacation
- On leave
- Temporarily unavailable
- Away from the office

The automatic reply informed senders that the employee was unavailable and directed urgent requests to the IT Support mailbox.

![Automatic Replies](Lab%20Microsoft365%20Administration/09-Automatic-Replies.png)

Automatic replies can either be manually enabled or configured for a specific date and time period.

---

# Phase 6 – Mail Forwarding

Email forwarding was configured for the employee mailbox.

Mail forwarding can be useful when:

- An employee is temporarily unavailable
- Responsibilities are transferred to another employee
- An employee leaves the organization
- Mail needs to be monitored by another authorized user

The configuration was tested by sending an email to the employee and verifying that the message was forwarded correctly.

![Mail Forwarding](Lab%20Microsoft365%20Administration/10-Mail-Forwarding.png)

---

# Phase 7 – Microsoft Teams Administration

A Microsoft Team named **IT Operations** was created.

The Team was configured as **Private**, meaning only authorized members could access it.

### IT Operations Team

![IT Operations Team](Lab%20Microsoft365%20Administration/11-IT-Operations-Team.png)

### Team Membership

The administrator was configured as the **Owner**.

John was configured as a **Member**.

This demonstrated the difference between administrative ownership and standard team membership.

![Team Members](Lab%20Microsoft365%20Administration/12-Team-Members.png)

---

## Help Desk Channel

A channel named **Help Desk** was created inside the IT Operations Team.

The channel was designed for:

- Troubleshooting discussions
- Internal IT communication
- Help desk coordination
- Technical support collaboration

![Help Desk Channel](Lab%20Microsoft365%20Administration/13-Help-Desk-Channel.png)

---

# Phase 8 – SharePoint Online

Creating the Microsoft 365 Team also created a connected SharePoint Team Site.

This demonstrated the integration between:

```text
Microsoft 365 Group
        |
        +---- Microsoft Teams
        |
        +---- SharePoint Online
        |
        +---- Shared Files
```

### SharePoint Active Site

The IT Operations SharePoint site was verified through the SharePoint Admin Center.

![SharePoint Active Site](Lab%20Microsoft365%20Administration/14-SharePoint-Active-Site.png)

### IT Operations SharePoint Site

![SharePoint Site](Lab%20Microsoft365%20Administration/15-SharePoint-Site.png)

---

## SharePoint Document Library

A test IT support document was uploaded to the SharePoint document library.

This demonstrated centralized team file storage.

![SharePoint Document](Lab%20Microsoft365%20Administration/16-SharePoint-Document.png)

The employee account was also used to confirm that members of the IT Operations Team could access the SharePoint resources.

---

# Phase 9 – OneDrive Administration

OneDrive was used to demonstrate personal cloud storage for an employee.

The key difference between OneDrive and SharePoint is:

```text
OneDrive
Personal employee work files

SharePoint
Shared team or organizational files
```

### Employee OneDrive

A test file was created in John's personal OneDrive.

![John OneDrive](Lab%20Microsoft365%20Administration/17-John-OneDrive.png)

---

## OneDrive File Sharing

The employee shared the OneDrive test file with the administrator.

The administrator successfully accessed the file.

Access was later removed to demonstrate permission revocation.

![OneDrive Sharing](Lab%20Microsoft365%20Administration/18-OneDrive-Sharing.png)

This demonstrated that OneDrive files remain private unless access is explicitly shared.

---

# Phase 10 – Password Reset

A common Help Desk scenario was simulated where an employee required a password reset.

Using the Microsoft 365 Admin Center, the employee password was reset and a temporary password was generated.

The employee was then required to change the password during the next sign-in.

![Password Reset](Lab%20Microsoft365%20Administration/19-Password-Reset.png)

This simulated the workflow:

```text
User reports password issue
        |
        v
Help Desk verifies user
        |
        v
Administrator resets password
        |
        v
Temporary password issued
        |
        v
User creates a new password
```

---

# Phase 11 – Sign-In Management

Microsoft 365 administrators can block a user's ability to sign in.

This is useful for:

- Employee termination
- Security incidents
- Compromised accounts
- Temporary account suspension

The sign-in control for the employee account was tested.

![Sign-In Control](Lab%20Microsoft365%20Administration/20-Sign-In-Control.png)

The account was later restored to confirm normal access before the final offboarding process.

---

# Phase 12 – Microsoft 365 Service Health

The Microsoft 365 Service Health dashboard was reviewed.

This is an important troubleshooting tool because an issue may be caused by a Microsoft service outage instead of a user's computer or account.

Administrators can check the health of services such as:

- Exchange Online
- Microsoft Teams
- SharePoint Online
- OneDrive
- Microsoft 365 services

![Service Health](Lab%20Microsoft365%20Administration/21-Service-Health.png)

Checking Service Health can prevent unnecessary troubleshooting when the problem is a Microsoft-side outage.

---

# Phase 13 – Employee Offboarding

The final phase simulated an employee leaving the organization.

Before offboarding, the employee account and existing access were reviewed.

![Account Before Offboarding](Lab%20Microsoft365%20Administration/22-Account-Before-Offboarding.png)

---

## Offboarding Procedure

The following actions were completed:

1. Blocked employee sign-in
2. Removed employee from the IT Operations Team
3. Removed employee from the Microsoft 365 Group
4. Removed employee from the IT TEAM distribution list
5. Removed shared mailbox permissions
6. Removed Read and Manage access
7. Removed Send As permissions
8. Removed Send on Behalf permissions
9. Removed the Microsoft 365 Business Premium license
10. Retained the user account instead of immediately deleting it

---

## Sign-In Blocked

The employee was prevented from accessing Microsoft 365 services.

![Sign-In Blocked](Lab%20Microsoft365%20Administration/23-Sign-In-Blocked.png)

---

## License Removed

Microsoft 365 Business Premium was removed from the employee.

This reclaimed the license so it could be assigned to another employee.

![License Removed](Lab%20Microsoft365%20Administration/24-License-Removed.png)

---

## Final Offboarding State

The employee account remained in Microsoft 365, but access was blocked and the Microsoft 365 license was removed.

![Final Offboarding](Lab%20Microsoft365%20Administration/25-Offboarding-Final.png)

This demonstrates that employee offboarding should not simply involve deleting an account immediately.

Organizations may need to preserve:

- Email
- OneDrive files
- Business records
- Audit information
- Organizational data

before permanently deleting an account.

---

# Troubleshooting Performed

Several troubleshooting scenarios were encountered during the lab.

## Shared Mailbox Access

After assigning shared mailbox permissions, the employee initially could not access the mailbox.

The following were verified:

- Read and Manage permissions
- Send As permissions
- Shared mailbox membership
- Outlook session
- Permission synchronization

After the permissions propagated, the shared mailbox became accessible.

---

## SharePoint Access

The employee initially encountered an error while navigating to SharePoint through the Microsoft 365 interface.

The following were checked:

- Microsoft 365 Group membership
- Teams membership
- SharePoint site membership
- Direct SharePoint site access

The employee successfully accessed the SharePoint site using the direct site URL, confirming that SharePoint permissions were configured correctly.

---

## Sign-In Troubleshooting

During testing, the Microsoft 365 license and sign-in status were changed.

When access was restored, the following were verified:

- Sign-in status was allowed
- Microsoft 365 Business Premium was reassigned
- User account remained active
- Authentication was tested using a private browser session

---

# Microsoft 365 Concepts Learned

This lab provided hands-on experience with several important Microsoft 365 concepts.

### Identity

Microsoft Entra ID provides the identity used to access Microsoft 365 services.

### Licensing

A Microsoft 365 user account can exist without having access to all Microsoft 365 services.

Licenses determine which services are available to the user.

### Exchange Online

Exchange Online provides cloud-based email and mailbox services.

### Shared Mailbox

A shared mailbox allows multiple authorized users to work from the same organizational email address.

### Distribution List

A distribution list sends a copy of an email to multiple members.

### Microsoft Teams

Teams provides communication and collaboration for departments and project groups.

### SharePoint

SharePoint provides centralized storage and collaboration for organizational and team files.

### OneDrive

OneDrive provides personal cloud storage for individual employees.

---

# Skills Practiced

Through this lab I gained hands-on experience with:

- Microsoft 365 Admin Center
- Microsoft 365 user administration
- User onboarding
- Microsoft 365 licensing
- Exchange Online administration
- Mailbox management
- Email aliases
- Shared mailboxes
- Mailbox delegation
- Send As permissions
- Distribution lists
- Automatic replies
- Mail forwarding
- Microsoft Teams administration
- Team ownership and membership
- Teams channels
- SharePoint Online
- SharePoint permissions
- Document libraries
- OneDrive
- File sharing permissions
- Password resets
- Account sign-in management
- Microsoft 365 Service Health
- User access troubleshooting
- Employee offboarding
- License reclamation

---

# Real-World Help Desk Scenarios Practiced

This lab simulated several common IT support tickets:

```text
"Please create an account for our new employee."

"I forgot my Microsoft 365 password."

"I cannot access Outlook."

"Please give me access to the IT Support mailbox."

"I need to send an email from the support mailbox."

"Please add me to the IT distribution list."

"I cannot access the IT SharePoint site."

"Please share this OneDrive file."

"Please configure an out-of-office message."

"Please forward this employee's email."

"This employee has left the company. Disable their access."
```

---

# Security Considerations

During the lab, administrative access was separated from standard employee access.

The employee account was configured without administrative privileges.

Sensitive information such as passwords and temporary credentials should never be stored in public GitHub repositories.

Screenshots used in this repository should not expose:

- Passwords
- Temporary passwords
- Recovery information
- Payment information
- Authentication secrets

---

# Lab Outcome

The Microsoft 365 Administration Lab successfully demonstrated the complete lifecycle of a Microsoft 365 employee account:

```text
Create User
     |
     v
Assign License
     |
     v
Configure Email
     |
     v
Configure Collaboration
     |
     v
Configure File Access
     |
     v
Provide Help Desk Support
     |
     v
Manage Security
     |
     v
Offboard Employee
     |
     v
Reclaim License
```

This lab provided practical experience with the Microsoft 365 administration tasks commonly performed by **Help Desk Technicians, IT Support Technicians, Desktop Support Technicians, and Junior System Administrators**.

---

## Lab Status

**Completed ✅**
