import pypandoc

markdown = """# License Reconciliation in Snipe-IT

**Purpose:** Ensure Snipe-IT license assignments match the organization's actual license records.

**Frequency:** Monthly  
**Reference Ticket:** [SR-58400](https://genzeonservicedesk.freshservice.com/helpdesk/tickets/58400)

## Step 1: Review the ticket
Open the monthly service ticket and identify the licenses to be reconciled.

## Step 2: Log in to Snipe-IT
Sign in using your authorized credentials.

![Snipe-IT login screen](https://github.com/user-attachments/assets/a29e4d7e-6f99-4d5f-b3f1-15cd487d3369)

## Step 3: Open Licenses
Go to **Licenses** and check the total and available license counts.

![Snipe-IT Licenses section](https://github.com/user-attachments/assets/e32670ec-456b-4c9a-86dc-2b1479e84a5b)

## Step 4: Check assignments
Open the relevant license (for example, **Adobe Inc**) and review assigned users. Use **Export** if you need the assignment details.

## Step 5: Reconcile licenses
- If a user has a valid license but it is not assigned in Snipe-IT, assign it.
- For terminated or inactive users, revoke the license in the actual vendor portal, then unassign it in Snipe-IT.
- If a Snipe-IT entry does not exist in the actual license records, validate and remove or correct the entry.

**Note:** Snipe-IT **Check In** only unassigns the license in Snipe-IT. It does not revoke the license in the vendor portal.

## Step 6: Assign a license
Select the correct user and click **Check Out**. Verify that the license appears under the user's assignments.

![Snipe-IT license assignment screen](https://github.com/user-attachments/assets/c7cae979-894c-4576-a9c5-ce833418876d)

## Final Check
- Confirm Snipe-IT matches the actual license records.
- Verify assigned and available license counts.
- Update the service ticket with the completed actions.
"""

output_path = "/mnt/data/License_Reconciliation_Snipe-IT_With_Pictures.md"
pypandoc.convert_text(markdown, "md", format="md", outputfile=output_path, extra_args=["--standalone"])
print(output_path)
