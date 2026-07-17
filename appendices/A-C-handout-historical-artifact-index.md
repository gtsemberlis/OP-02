---
object_uuid: 81eb1386-dcf8-528d-9199-e4d0bbaeec40
canonical_reference: A-C
object_type: Appendix
title: Handout / Historical Artifact Index
publication: OP-01
schema_version: '1.0'
content_version: '1.0'
publication_status: Published
last_revised: '2026-07-16'
revision_note: Appendix C canonical population
source_path: appendices/A-C-handout-historical-artifact-index.md
tags: []
related_objects:
- H-01
- H-03
- H-04
- H-05
- H-09
- H-08
- H-07
- H-06
- A-01
- A-02
- A-03
- A-04
- A-05
- A-06
- A-07
- A-08
- A-09
---

# A-C — Handout / Historical Artifact Index

## Purpose

Provide separate production and running indexes for canonical operational Artifacts and player-facing Handouts. Artifact records govern custody, discovery, access, and investigative significance. Handout records contain the complete in-world documents or facsimiles that may be given to players.

## Canonical Content

### Player Handouts

| Reference | Handout | Related Artifact | First Appearance | Default Presentation |
|---|---|---|---|---|
| H-01 | FAA Initial Incident Summary | A-02 — O'Hare Incident Summary | S-01 — Cold Open: O'Hare Hard Landing | Restrained federal incident document |
| H-03 | Alexandria Technical Information Brief | A-03 — Alexandria Technical Overview | S-04 — Alexandria Systems Review | Corporate engineering brief |
| H-04 | NTSB Witness Briefing Sheets | None — administrative briefing packet | S-06 — Independent Witnesses | Five separate NTSB briefing sheets |
| H-05 | Rao's Research Notebook | A-05 — Dr. Rao's Research Notebook | S-05 — Independent Analysis | Ten notebook pages plus inside back cover |
| H-06 | Rao's Comparative Incident Timeline | A-04 — Runway Obstruction Event Summary | S-05 — Independent Analysis | Internal chronological engineering working document |
| H-07 | Collector Field Notes | A-07 — Collector Notebook Fragments | S-07 — Competing Observers | Eight recovered handwritten notebook fragments |
| H-08 | Owen Walker's Drawing | A-06 — Owen Walker's Drawing | S-06 — Independent Witnesses | Full-page image facsimile |
| H-09 | Comparative Case File | A-09 — Comparative Case File | S-09 — Inheritance | Restrained Program reference file and case index |

### Operational Artifacts

| Reference | Artifact | Artifact Type | First Appearance | Player Handout |
|---|---|---|---|---|
| A-01 | Initial Program Briefing | Operational briefing document | S-01 — Initial Assignment | Not yet restored |
| A-02 | O'Hare Incident Summary | Official aviation incident summary | S-01 — Cold Open: O'Hare Hard Landing | H-01 |
| A-03 | Alexandria Technical Overview | Corporate technical briefing | S-02 — Alexandria Headquarters | Not yet restored |
| A-04 | Runway Obstruction Event Summary | Alexandria internal incident chronology | S-04 — Alexandria Internal Investigation | Not yet restored |
| A-05 | Dr. Rao's Research Notebook | Handwritten scientific research notebook | S-03 — Dr. Ananya Rao | Not yet restored |
| A-06 | Owen Walker's Drawing | Civilian drawing / observational artifact | S-06 — Witness Interviews | Not yet restored |
| A-07 | Collector Notebook Fragments | Recovered field notebook / historical artifact | S-07 — The Collectors | Not yet restored |
| A-08 | Alexandria Runway Observation Record | Controlled experiment record | S-08 — Runway Observation | Not yet restored |
| A-09 | Comparative Case File | Program comparative analysis file | S-09 — Comparative Assessment & Debrief | Not yet restored |

## Source Objects

Artifact reference records are stored in `artifacts/` using the `A-##` namespace. Complete player-facing documents are stored in `handouts/` using the `H-##` namespace.

Current canonical handout sources:

- `handouts/H-01-faa-initial-incident-summary.md`
- `handouts/H-03_Alexandria_Technical_Information_Brief.md`
- `handouts/H-04-ntsb-witness-briefing-sheets.md`
- `handouts/H-05_Raos_Research_Notebook.md`
- `handouts/H-06_Raos_Comparative_Incident_Timeline.md`
- `handouts/H-07_Collector_Field_Notes.md`
- `handouts/H-08_Owen_Walker_Drawing.md`
- `handouts/H-09_Comparative_Case_File.md`

This appendix is an index only. Individual Artifact and Handout files remain authoritative.

## GM Guidance

Prepare only Handouts the investigators have earned access to. Do not distribute an Artifact record as though it were an in-world document. Player-facing presentation should support credibility without announcing supernatural importance.

## Refresh Rule

Regenerate this appendix whenever an Artifact or Handout is added, removed, renamed, linked, or assigned a different first appearance.
