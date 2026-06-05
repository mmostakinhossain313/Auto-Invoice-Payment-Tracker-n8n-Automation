# Invoice Number Note

I generate unique invoice numbers automatically.

Formula I use:
INV-{{ $json['Email Address'].split('@')[0] }}-{{ $now.toFormat('yyyyMMddHHmmss') }}

Example output:
INV-john-20260605162134

Why this works:
- Email username makes it personal
- Timestamp makes it unique
- Combined = always different for every client

One mistake I made:
I used only timestamp at first.
Two orders in the same second got same invoice number.
Fix: Added email username to make it truly unique.
