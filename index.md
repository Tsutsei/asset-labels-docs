---
layout: page
title: Overview
permalink: /
---

**Asset Labels – Bulk QR Labels for Jira Assets** prints QR code labels for your Jira Service Management Assets objects – hundreds at once, with the fields you choose, on standard label sheets or on a label printer.

Assets itself prints one QR code with the object key. When you need to label 300 laptops with their serial number, location and "Property of …", you need more. Asset Labels:

- **Finds the objects** – choose an object schema and type, narrow it down with AQL (for example `Location = "Prague"` or `Status = "In stock"`), tick or untick objects.
- **Designs the label** – title, up to three attribute lines, a footer, and what the QR code contains (a link to the object in Jira, the key, or any attribute). A live preview shows the label as it prints.
- **Prints it** – PDF for A4 and Letter label sheets (Avery) and for label printers, ZPL for Zebra printers. Start in the middle of a partly used sheet.
- **Remembers the design** – save templates that everyone on the site can use.

Scan a label with a phone and the object opens in Jira.

## Safe by design
- Assets data is read **with the user's own permissions**, in the browser. Labels are created there too – the app never stores or sends Assets data anywhere.
- The app only **reads** Assets. It never changes objects.
- It stores only label templates, no personal data. **Runs on Atlassian.**

## Requirements
Jira Service Management **Premium or Enterprise** with Assets, and access to the object schemas you want to label.

Start with the [user guide]({{ '/guide/' | relative_url }}) or check the [label sizes]({{ '/sizes/' | relative_url }}).
