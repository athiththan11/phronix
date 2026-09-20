---
layout: default
title: Open Data
description: The merchant location database used by Phronix, published under the Open Database Licence (ODbL).
---

## Merchant locations

Phronix uses a list of merchant branch locations to show which of your card offers are near you. That list is derived from OpenStreetMap data, so it is published here under the licence it was derived under.

**Download:** [merchant-locations.json]({{ '/open-data/merchant-locations.json' | relative_url }})

---

## Licence and attribution

This database contains information from **OpenStreetMap**, which is made available under the [Open Database Licence (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/). © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright).

The Phronix merchant location database is a derivative of that data and is also made available under the ODbL 1.0. You may copy, distribute, and adapt it, provided that you credit OpenStreetMap contributors, keep this notice, and offer any adapted version you publicly use under the ODbL as well. The full licence terms are in the link above.

---

## What was changed

The database starts from OpenStreetMap points of interest in Sri Lanka and:

- matches them to the merchants named in bank card offers, using name matching with a confidence threshold;
- keeps a location for each merchant branch that matched;
- adds manual corrections and additions (entries whose `source` is `override`), which are offered under the same licence.

---

## Fields

| Field | Meaning |
|---|---|
| `id` | `osm:<type>/<id>` names the OpenStreetMap object an entry came from (for example `osm:way/173114261`); `manual:<name>` marks an entry Phronix created or corrected |
| `merchant` | Merchant name as it appears in bank offers |
| `branch` | Branch name, where known |
| `lat`, `lon` | Latitude and longitude in decimal degrees (WGS 84) |
| `source` | `osm` for entries taken from OpenStreetMap, `override` for manual entries |

The file also carries `version` and `generatedAt` (the UTC time it was built), `attribution`, and `license`.

---

## Accuracy

This data is provided as is. Locations can be wrong or out of date. To correct a place at its source, edit it on [openstreetmap.org](https://www.openstreetmap.org/); corrections there flow into later versions of this database.

---

## Contact

Questions about this data: [athiththan.kathir@gmail.com](mailto:athiththan.kathir@gmail.com).
