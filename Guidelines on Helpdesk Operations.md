# Guidelines on Helpdesk Operations

**SOP Description:** Explains About the Helpdesk Operations.

## 1. Purpose

This SOP defines how service requests, incidents, and user queries are handled, tracked, communicated, and resolved in order to maintain business continuity across the organization.

## 2. Scope

This SOP applies to all Helpdesk activities related to IT support services. It covers:

- Incident management
- Service request fulfillment (e.g., password resets, software installations, account provisioning)
- Hardware and software troubleshooting
- User onboarding and offboarding support
- Access and permissions requests
- Device allocation and asset tracking

## 3. Ticket Logging & Processing

- We receive Auto assigned Ticket to the Board then we check the Ticket for the requested.
- Log incidents/requests with required user and issue details.
- Categorize and prioritize based on impact and urgency.
- Capture device/app details, error info, and attachments if available.

### 3.1 Initial Diagnosis

- Perform troubleshooting to identify the issue.

### 3.2 Investigation & Resolution

- The auto-assigned ticket team member investigates and writes the root cause (RCA).
- Communication is maintained with the end user during the process.

### 3.3 User Verification & Closure

- The final ticket status is shared with the user for confirmation.
- Once verified, or after a defined period of inactivity, the ticket is closed.
- Resolution notes and RCA details are documented for future reference.

## 4. Communication Standards

The Helpdesk communicates with users through approved channels such as:

- IT Service Portal
- Email

Communication must include:

- Ticket acknowledgement
- Work in progress / awaiting information updates
- Resolution notification

## 5. Tools & Platforms

The Helpdesk uses Freshservice as the primary platform for raising and managing tickets.

### 5.1 Remote Support Tools

Used for remote troubleshooting, device access, and diagnostics.

- ManageEngine

### 5.1 Communication Tools

Used for internal and user communication via:

- Email
- Microsoft Teams

## 6. Asset Management

- We use Snipe-IT for Tracking of devices and Inventor.

## 7. Onboarding & Access Requests

### 7.1 New Employee Onboarding

During employee Onboarding, we receive a CSV from P&C Team and we need to throughly check the CSV then we proceed if we find any errors we need to recheck With P&C Team then we need to Run the PowerShell script for Onboarding the User and User account Creation.

**Responsibilities include:**

- User account creation (AD / Azure)
- Email and collaboration access.
- IT Asset allocation (Laptop, Headset, Charger, Joining Kit)

### 7.2 Access Requests

Users may request:

- Application access
- Shared folder permissions
- Admin/privileged access (requires approvals)
- Remote/VPN access

All access requests must follow organizational access control policies and requires:

- Manager approval
- Compliance validation (for privileged roles)

## 8. Offboarding & Access Removal

During employee exit, we receive a CSV from P&C Team then we proceed to Run the PowerShell script for offboarding the User and User account removing.

- Disable accounts and revoke Biometric access
- Recover hardware assets
- Reassign shared data or mailboxes if needed
- Remove licenses
