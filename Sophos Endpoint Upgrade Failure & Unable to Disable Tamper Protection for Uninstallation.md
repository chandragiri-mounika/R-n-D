# Sophos Endpoint Upgrade Failure & Unable to Disable Tamper Protection for Uninstallation

## SOP Description

Explains About how to Unable to Disable Tamper Protection for Uninstallation.

## 1. Purpose:

The purpose of this is to Safely disable Sophos Tamper protection on Windows Endpoint for Uninstallation of Sophos Endpoint Agent. This process helps to Enables to regain the control of the system for trouble-shooting of Sophos Components from Device.

### 1. Scope:

This procedure applies to Windows Devices.

### 2. Responsibilities:

- Execute the procedure as per the SOP.
- Ensure administrative access credentials are available.
- Perform registry backup before Modify.

### 3. Procedure:

**Tamper protection in the registry.**

Do the Following Recovery steps.

**Windows10 and later and windows**

1. For Windows 10, and windows later., go to settings, Update, &security, recovery under Advanced start-up click Restart Now.

2. Restart to recovery by holding the shift key on your keyboard, clicking power, and then clicking Restart.

3. It will appear with bitlocker key recovery. Then go> Intune> select Devices> Windows> Then try to search by Asset Tag.

4. Then try to share the Key with user then click on Continue then you will be able to see two options click on Troubleshooting. Then it will open with advanced options click on Command prompt.

5. After the restart, select an administrative account to continue and enter the password.

   a. Open Command Prompt.

   b. Type C: and press Enter.

   **Note:** Your Boot drive may differ from C. If so, use a command such as DiskPart and list volume to show the available volumes.

   c. Type cd Windows\System32\drivers and press Enter.

   d. Type ren SophosED.sys SophosED.sys.old and press Enter.

   e. Type exit and press Enter.

   f. Click Continue.

   g. Once back in Windows, open Registry Editor.

   h. Back up the registry. By going to files at left bottom to files and Export the Files to Desktop drive.

   i. Then Go to HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\Sophos Endpoint Defense\TamperProtection\Services and under every subkey in this location, set the Value data of Protected to 0.

   j. Example: Go to HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\Sophos Endpoint Defense\TamperProtection\Services\hmpalert and set the Value data of Protected to 0.

   k. Then Go to HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\Sophos Endpoint Defense\TamperProtection\Config and set the Value data of SEDEnabled to 0.

   l. Then restart the Device.

   m. Then share the Zap file with user which is provided in Document.

   n. Download SophosZap.

   o. Right-click SophosZap.exe.
      i. Select Properties.
      ii. Check File version in the Details tab.

   p. Then open the Command Prompt With Admin privilges.

   q. Try to change the path to the current location of SophosZap.exe.

   r. Then type Sophos and hit Tab button while the SophosZap.exe found.

   s. Run the command SophosZap --confirm.

   t. Then you will see the Message saying Reboot and re-excute once SophosZap has completed its first steps.

   u. Then try to restart as shown.

   v. Once's it shows the message saying Uninstallation.

   w. Then proceed for uninstallation going to Control panel.

   x. Then again try to re-install the Sophos XDR using the Self- service portal. Or try using the mentioned link https://missa.genzeon.com/mis/sophosxdr.exe

   y. After the successfully installation of the Sophos XDR go to about and try to click on Update.

   z. Then try to check in the Sophos that now its visible or not.

## Image Reference

![Sophos Endpoint Upgrade Failure and Tamper Protection Recovery](https://github.com/user-attachments/assets/06eb6046-6dde-43d0-b9bd-1f0897af4c3a)
