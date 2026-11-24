# Handling Common Microsoft Teams and Outlook Issues

**SOP Description:** Explains About the Common Microsoft Teams and Outlook Issues.

## 1. Purpose

This SOP outlines the standardized process for identifying, troubleshooting, and resolving common day-to-day issues faced in Microsoft Teams and Microsoft Outlook.

## 2. Scope

This procedure applies to all IT support engineers handling user-reported issues related to Teams and Outlook within the organization.

## 3. Responsibilities

- **IT Support Engineer:** Troubleshoot and resolve issues following this SOP.
- **User:** Provide required information and allow remote access when needed.

## 4. Procedure

### A. Microsoft Teams – Issue Handling

#### 1. Login / MFA Issues

**Common Causes:** Incorrect credentials, MFA delays, system time mismatch.

**Steps:**

1. Verify username and password with the user.
2. Check internet connectivity.
3. Ensure system date/time is set to automatic.
4. Ask user to retry MFA or resend OTP.
5. If still failing, reset MFA or raise to Security/Identity team.

#### 2. Teams Not Syncing / Messages Delayed

**Steps:**

6. Verify network status.
7. Sign out and sign in from Teams.
8. Clear Teams cache:

```text
%AppData%/Microsoft/Teams → Delete contents.
```

9. Restart system.

#### 3. Unable to Join/Host Meetings

**Steps:**

10. Check if Teams is updated.
11. Verify meeting permissions.
12. Ensure camera/mic permissions are enabled in Windows privacy settings.
13. Reinstall Teams if required.

#### 4. Audio/Video Issues

**Steps:**

14. Check if correct mic/speaker/camera is selected in Teams.
15. Test devices in "Settings → Devices".
16. Check if any other app is using the camera.
17. Update audio/video drivers.

#### 5. Teams Add-in Missing in Outlook

**Steps:**

18. Open Outlook → File → Options → Add-ins.
19. Enable Microsoft Teams Meeting Add-in.
20. Restart Outlook.
21. If missing, repair Office.

#### 6. File Upload/Download Issues

**Steps:**

22. Check SharePoint/OneDrive permissions.
23. Verify storage quota.
24. Test on web version.

---

### B. Outlook – Issue Handling

#### 1. Outlook Not Opening / Crashing

**Steps:**

25. Open Outlook in safe mode:

```cmd
outlook.exe /safe
```

26. Disable suspicious add-ins.
27. Create new Outlook profile.
28. Repair Office.

#### 2. Unable to Send/Receive Emails

**Steps:**

29. Check network connectivity.
30. Verify mailbox storage.
31. Review mailbox rules.
32. Sync mailbox or recreate profile.

#### 3. Search Not Working

**Steps:**

33. Rebuild search index.
34. Ensure Windows Search service is running.
35. Repair OST file.

#### 4. Calendar Sync Issues

**Steps:**

36. Ensure Teams add-in is enabled.
37. Update Outlook.
38. Reconnect mailbox.

#### 5. PST/OST Corruption Issues

**Steps:**

39. Create new OST by removing old one.
40. Recreate profile if needed.
