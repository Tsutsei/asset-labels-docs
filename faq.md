---
layout: page
title: FAQ
permalink: /faq/
---

**Which plans does it need?**
Jira Service Management Premium or Enterprise – Assets is part of these plans.

**Who can print labels?**
Everyone who can see the objects in Assets. The app reads Assets with each user's own permissions.

**Does the app change my assets?**
No. It only reads object schemas, types, attributes and objects.

**Where are the labels created? Is my data sent anywhere?**
In your browser. PDF and ZPL files are created there and downloaded by you; Assets data is never sent to or stored by the app.

**How many labels at once?**
1 000 objects per batch; **Load the next 1 000** continues with the following ones. Add `ORDER BY` to the filter to control the order.

**Which characters are supported?**
All European characters (for example č, ł, ø, ß, ő) – the PDF embeds the DejaVu Sans font. ZPL is sent as UTF-8; your Zebra printer needs a font with these characters.

**What does the QR code open?**
With "Link to the object in Jira", the object's page in Assets – the person scanning needs access to Assets on your site. You can also put the key or any attribute (for example a serial number) into the QR code.

**Can I add a logo?**
Yes – a PNG or JPG up to 150 kB, saved with the template. It is printed in PDFs (not in ZPL).

**QR code or barcode?**
QR codes are read by phones and can hold a link that opens the object. Code 128 barcodes are read by handheld barcode scanners and hold up to 48 plain characters, for example the key or a serial number.

**Can I use my own label software?**
Yes – **Download CSV** gives the code content and the texts of every label, ready for BarTender, P-touch Editor and similar tools.

**What happens to templates when I uninstall?**
They are deleted with the app's data.
