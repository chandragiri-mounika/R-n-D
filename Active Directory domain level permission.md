# Active Directory – Domain-Level Permission

## Purpose
To allow a user to update Active Directory user accounts without granting full **Domain Admin** privileges using the Delegation of Control Wizard.

## Steps to Delegate Permissions

### Step 1: Open ADUC
- Open **Active Directory Users and Computers (ADUC)**.
- Locate the `corp.local` domain.

### Step 2: Delegate Control
- Right-click `corp.local`.
- Select **Delegate Control**.

![Delegate Control](https://github.com/user-attachments/assets/6c7dba99-6d75-4062-b245-2645468655a7)

### Step 3: Add User
- Click **Next**.
- Click **Add**.
- Search for the required username.
- Click **Check Names → OK → Next**.

### Step 4: Select Permissions
Choose one of the following:
- **Delegate the following common tasks**
- **Create a custom task to delegate**

Select the required option and click **Next**.

### Step 5: Finish
- Review the selected permissions.
- Click **Finish**.

**Result:** The user receives the delegated permissions.

## Remove Delegated Permissions

1. Open ADUC.
2. Navigate to the domain or OU where permissions were delegated.
3. Right-click and select **Properties**.
4. Open the **Security** tab.
5. Select the user and remove the applicable delegated permissions.
6. Click **Apply → OK**.

**Note:** Verify permissions and inheritance before removing entries. Follow the Principle of Least Privilege and obtain approval before making changes.
