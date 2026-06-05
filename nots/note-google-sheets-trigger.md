# Google Sheets Trigger Note

I use Google Sheets Trigger when a Google Form submits data.

The trigger watches the sheet 24/7.
The moment a new row appears, the workflow starts.

Important setting:
Event = Row Added

One mistake I made:
I used regular Google Sheets node instead of Trigger.
The workflow never started automatically.
Always use Google Sheets Trigger for form responses.
