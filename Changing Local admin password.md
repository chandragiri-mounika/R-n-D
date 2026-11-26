
# Changing Local Admin Password

## SOP Description

Change the local administrator password after the user's laptop has been configured.

There are two methods to change the local administrator password:

1. ManageEngine Endpoint Central
2. Command Prompt or PowerShell

---

## Method 1: ManageEngine Endpoint Central

### Prerequisites

- Ensure you have access to ManageEngine Endpoint Central.
- Ensure the target laptop is configured and registered in Endpoint Central.
- Retrieve the approved local administrator password from Bitwarden.

### Procedure

**Step 1: Open Endpoint Central**

Log in to ManageEngine Endpoint Central and navigate to the home page.

**Step 2: Navigate to Computers**

Go to:

`Agents → Computers`

**Step 3: Search for the Computer**

- Enter the laptop's Asset Tag in the computer search field.
- Locate and select the respective computer.

**Step 4: Verify Agent Status**

Confirm that the Endpoint Central agent is online.

- Green status indicates that the agent is online.
- Ensure the agent is online before proceeding.

**Step 5: Open Command Prompt**

Navigate to:

`System Manager → Command Prompt`

**Step 6: Execute the Password Change Command**

Enter the following command:

```cmd
net user mis "#########"
```

Replace `#########` with the approved local administrator password retrieved from Bitwarden.

Execute the command.

**Step 7: Verify the Command Execution**

- Check the command output.
- Confirm that the command executed successfully.
- If an error occurs, investigate before proceeding.

---

## Method 2: Command Prompt or PowerShell

### Procedure

**Step 1: Open an Administrator Terminal**

- Log in to the target laptop using an authorized account.
- Open Command Prompt or PowerShell.
- Select **Run as administrator**.

**Step 2: Execute the Password Change Command**

Run the following command:

```cmd
net user mis "#########"
```

Replace `#########` with the approved local administrator password retrieved from Bitwarden.

**Step 3: Verify the Command Execution**

- Execute the command.
- Verify the command output.
- Confirm that the local administrator password was changed successfully.

---

## 3. Reference Screenshot

The following screenshot illustrates the local administrator password change procedure.

![Changing Local Admin Password](https://github.com/user-attachments/assets/554f43aa-13f8-4b25-89c5-e8fa58ec2ccf)

---

## 4. Important Notes

- Always retrieve the approved password from Bitwarden.
- Do not share or store local administrator passwords in plain text.
- Ensure the correct laptop is selected before executing the command.
- Verify the command execution before closing the task.
- Never include the actual password in tickets, screenshots, or SOP documentation.

## 5. Expected Result

The local administrator account (`mis`) password is successfully updated after laptop configuration.
