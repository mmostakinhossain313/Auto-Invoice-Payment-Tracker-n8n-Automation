# Field Names Note

Google Form field names have spaces.
In n8n expressions I must use brackets.

Correct way:
{{ $json['Client Name'] }}
{{ $json['Email Address'] }}
{{ $json['Service/Product'] }}
{{ $json['Amount'] }}

Wrong way:
{{ $json.Client Name }} — this breaks
{{ $json.Email Address }} — this breaks

Rule:
If field name has space = use ['Field Name']
If field name has no space = use .fieldname

This applies to Google Sheets, Google Forms, and any data with spaces in field names.
