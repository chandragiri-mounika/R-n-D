# Sophos Central – Device Policy Check

## 1. Purpose

This SOP outlines the procedure for verifying and ensuring that user devices are protected under the Sophos Central Security Policy and comply with organizational protection standards.

## 2. Scope

This procedure applies to all endpoints (laptops and desktops) within the organization managed under the Genzeon (GZN) Sophos Central Policy.

## 3. Responsibilities

- **IT / Security Team:** Responsible for verifying Sophos protection, scanning devices, and ensuring policy compliance.
- **End Users:** Must cooperate during the verification and scanning process.

## 4. Procedure Steps

### Step 1: Ticket Acknowledgement

- Receive a service ticket indicating that a user device is not protected by Sophos Central.
- Prioritize the ticket as **High**.
- Assign the ticket to the appropriate IT/Security support member.

### Step 2: User Communication

- Contact the user via Microsoft Teams or email to schedule a remote session.
- Request the user to keep the system powered on and connected to the internet.

### Step 3: Device Verification

- Connect to the user's device remotely.
- Open Sophos Endpoint Agent and check the protection status.
- Verify that the following features are active:
  - Real-Time Protection
  - Web Protection
  - Malware Scan
- Check whether the device is listed under the GZN Sophos Central Policy.

### Step 4: Run Initial Sophos Scan

- Perform a **Full System Scan** using Sophos Endpoint.
- Monitor the scan progress.
- Record any malicious or suspicious detections.

### Step 5: Remediation

- If malicious files are detected, use Sophos to quarantine and remove the detected threats.
- Restart the system if prompted.
- Record the remediation actions performed.

### Step 6: Post-Remediation Verification

- Run a second Full System Scan to ensure that no further malicious files are present.
- Confirm that the device status shows **Protected** in Sophos Endpoint.

### Step 7: Policy Verification

- Log in to the [Sophos Central Admin Console](https://central.sophos.com).
- Confirm that the device appears under the GZN Device Policy.
- Verify that the device complies with all required protection settings.

### Step 8: Documentation and Ticket Closure

- Update the service ticket with:
  - Initial scan results.
  - Detected threats, if any.
  - Remediation actions performed.
  - Post-remediation scan results.
  - Sophos policy verification status.
- Attach relevant screenshots or logs, if required.
- Close the ticket after successful verification.

## 5. References

- [Sophos Central Admin Portal](https://central.sophos.com)
