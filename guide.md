---
layout: page
title: User guide
permalink: /guide/
---

## Where to find it
In Jira: **Apps → Asset Labels**. Everyone with access to Assets can use it.

## 1. Choose the assets
1. **Object schema** and **Object type** – you see the schemas and types you can see in Assets.
2. **Filter (optional)** – an AQL condition that is combined with the object type, for example:
   - `Location = "Prague – 2nd floor"`
   - `Key in (ITH-1, ITH-2, ITH-3)`
   - `Status = "In stock" AND Created > now(-7d)`
   - add `ORDER BY` to choose the print order, e.g. `Location = "Brno" ORDER BY Key`
3. **Find assets**. 1 000 objects are loaded at a time; with more matches, print the first batch and then **Load the next 1 000**. All found objects are selected – untick the ones you do not need.

Object types are shown in their hierarchy with the number of objects; group (abstract) types cannot be chosen – choose one of their types.

## 2. Design the label
- **Label size** – a sheet (A4 or Letter), a label printer size, or **Label printer – custom size** with your own width and height (15–150 mm). See [label sizes]({{ '/sizes/' | relative_url }}).
- **Title** – the object name, the key or any attribute, printed in bold.
- **Line 1–5** – attributes printed below the title, the object name, or **Custom text…** – your own text such as "Do not remove" (as many lines as fit on the label size). With **Show attribute names** a line reads "Serial number: SN123"; when it does not fit, the font gets smaller, then the name is left out so the value stays readable.
- **Code** – a **QR code** (for phones) or a **Code 128 barcode** (for handheld barcode scanners), and what it **contains**: a **link to the object in Jira** (scan it to open the object), a **custom URL** – for example your service portal, with `{key}`, `{id}`, `{name}` and `{site}` filled in per object (`https://your-site.atlassian.net/servicedesk/customer/portal/1?asset={key}`) – the key, an attribute such as the serial number, or no code. Barcodes hold up to 48 plain characters and can print their text underneath.
- **Code size** – small, normal or large.
- **Text size** – small, normal, large or extra large, for labels that must be read from a distance.
- **Footer** – a short text at the bottom of every label, for example "Property of ACME · IT help: ext. 1234".
- **Logo** – a PNG or JPG (up to 150 kB), printed at the top right. Saved with the template.

The **preview** shows the first selected object as it will print.

## Templates
Give the design a **name** and **Save template**. Everyone on the site sees saved templates in the **Template** list; choosing one restores the size, fields, footer and logo (and its object type when it is in the chosen schema). Templates are shared, so changes are safe to undo:
- **Undo last change** brings back the version before the last save.
- **Delete template** removes it for everyone; **Restore deleted template** brings it back within 30 days.

## 3. Download
- **Skip used labels** – on sheets, leave the first labels empty when you print on a sheet that is partly used.
- **Copies per asset** – 1 to 10 labels per object (for example one for the device and one for its box).
- **Move right / Move down** – shift everything by up to 10 mm when your printer prints off-centre. Tick **Print label outlines** and print on plain paper first: hold the sheet against the labels to see the shift you need.
- **Download PDF** – print it at **100 % / actual size** (not "fit to page"), on the label stock that matches the size you chose.
- **Download ZPL (Zebra)** – for label printer sizes; send the file to a Zebra printer (for example with Zebra Setup Utilities or `lp -o raw`). ZPL labels have no logo.
- **Download CSV** – the code content and the texts of every label, for label software such as BarTender, P-touch Editor or Avery Design & Print.

Tip: print one sheet on plain paper first and hold it against the label sheet to check the alignment.
