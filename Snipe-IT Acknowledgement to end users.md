
## Prerequisites

- Add the user and assign the required assets in Snipe-IT.
- Click the below link to know how to add a user and update asset details:

**Reference:** [Update in Snipe-IT (Web View)](ADD_YOUR_REFERENCE_LINK_HERE)

## Procedure

### Step 1: Import the SnipeITOps Module

To send Snipe-IT acknowledgement emails to end users, we need to import the `SnipeITOps` PowerShell module.

Run the following cmdlet in PowerShell:

```powershell
Import-Module SnipeITOps -Verbose
```

### Step 2: Trigger the Acknowledgement Email

After importing the module, run the following cmdlet to trigger the acknowledgement email to the respective user:

```powershell
Send-SITITAssetAcknowledgementEmail -UPN <email Address>
```

**Example:**

```powershell
Send-SITITAssetAcknowledgementEmail -UPN user@company.com
```

Replace `user@company.com` with the actual email address of the end user.

### Step 3: Acknowledgement Email

After executing the cmdlet, the user will receive an acknowledgement email containing the details of their assigned assets.

The user will receive an email similar to the example below:

![Snipe-IT Acknowledgement Email](https://github.com/user-attachments/assets/f6f88d87-1041-4bfa-889a-688ad44dc543)
