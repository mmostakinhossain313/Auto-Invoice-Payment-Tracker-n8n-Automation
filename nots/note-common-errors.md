# Common Errors I Faced — Auto Invoice Tracker

Error 1: All invoices had same Invoice Number
Reason: Used timestamp only — same second = same number.
Fix: Combined email username + timestamp.

Error 2: Invoice details not saving to Sheet
Reason: Google Sheets Trigger only reads, does not write.
Fix: Added separate Google Sheets Update Row node.

Error 3: Expression showing undefined
Reason: Field name has space, used wrong expression format.
Fix: Use {{ $json['Field Name'] }} for fields with spaces.

Error 4: Client not receiving invoice email
Reason: Used my own email in To field instead of client email.
Fix: Use {{ $json.email }} in To field.

Error 5: Workflow not triggering
Reason: Workflow not published.
Fix: Always click Publish before testing.
