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
3. **Find assets**. Up to 1 000 objects are loaded at a time; narrow the filter to print more in batches. All found objects are selected – untick the ones you do not need.

## 2. Design the label
- **Label size** – a sheet (A4 or Letter) or a label printer size. See [label sizes]({{ '/sizes/' | relative_url }}).
- **Title** – the object name, the key or any attribute, printed in bold.
- **Line 1–3** – attributes printed below the title. With **Show attribute names** a line reads "Serial number: SN123"; when it does not fit, the font gets smaller, then the name is left out so the value stays readable.
- **QR code contains** – a **link to the object in Jira** (scan it to open the object), the key, an attribute, or nothing.
- **Footer** – a short text at the bottom of every label, for example "Property of ACME · IT help: ext. 1234".
- **Skip used labels** – on sheets, leave the first labels empty when you print on a sheet that is partly used.

The **preview** shows the first selected object as it will print.

## Templates
Give the design a **name** and **Save template**. Everyone on the site sees saved templates in the **Template** list; choosing one restores the size, fields and footer (and its object type when it is in the chosen schema). **Delete template** removes it for everyone.

## 3. Download
- **Download PDF** – print it at **100 % / actual size** (not "fit to page"), on the label stock that matches the size you chose.
- **Download ZPL (Zebra)** – for label printer sizes; send the file to a Zebra printer (for example with Zebra Setup Utilities or `lp -o raw`).

Tip: print one sheet on plain paper first and hold it against the label sheet to check the alignment.
