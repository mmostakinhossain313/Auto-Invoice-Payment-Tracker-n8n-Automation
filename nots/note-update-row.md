# Google Sheets Update Row Note

Google Sheets Trigger only reads data.
It does not write anything back to the sheet.

To save Invoice No, Date and Status I need:
A separate Google Sheets node with Operation = Update Row.

Settings I use:
- Operation: Update Row
- Column to Match: Email Address
- Fields to Update: Invoice No, Date, Status

One mistake I made:
I thought Trigger would save data automatically.
Sheet had no Invoice No or Status.
Fix: Added Update Row node after Gmail node.
