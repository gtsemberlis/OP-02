# Source Edition Schema v1.0 (Frozen)

Status: **FROZEN** for OP-01 Source Edition v1.0.

Every object uses the global envelope fields present in each file. Required content sections are represented as level-two headings. Optional or conditional sections are explicitly labeled.

## Object contracts

| Type | Required content sections |
|---|---|
| Scene | Chapter; Scene Summary; Scene Purpose; Primary Location(s); Participants; Estimated Runtime; Investigation Phase; Scene Flow; Key Information; Evidence Available; Likely Investigator Approaches; GM Guidance; Before Leaving This Scene; Quick Reference; Related Objects; Prerequisites (Optional); Variant Paths (Optional) |
| Npc | Affiliation; Position / Occupation; Primary Location; Current Status; Personnel Record; Physical Description; Operational Role; Biography; Private Context; Cognitive Signature; Communication Style; Under Pressure; Investigative Utility; Operational Knowledge; Relationships; Post-Operation Status; Operational Notes; Mechanical Reference; Related Objects |
| Location | Owner / Responsible Organization; Accessibility; Operational Status; Overview; Operational Function; Environmental Characteristics; Associated NPCs; Associated Artifacts; Associated Scenes; Operational Notes |
| Artifact | Artifact Type; Current Custody; Current Location; Custody History; First Appearance; Related Scenes; Related NPCs; Related Locations; Description; Canonical Content; Presentation Notes; Investigator Access Conditions; Operational Significance; Preservation Notes; Related Handouts (Optional) |
| Handout | Document Type; In-World Author; Player Version; GM Annotation; Related Artifact; Distribution Conditions; Presentation Notes |
| Handler Tool | Purpose; Canonical Sources; Use at the Table; Derived Content; Refresh Rule |
| Appendice | Purpose; Canonical Content; Source Objects; GM Guidance; Refresh Rule |

## Controlled vocabularies

- Publication status: Draft, Review, Canonical, Deprecated
- Object type: Publication, Front Matter, Scene, NPC, Institution, Location, Artifact, Handout, Handler Tool, Appendix
- Operation classification: Blue, Yellow, Orange, Red, Black
- Accessibility: Public, Controlled, Restricted, Program-Only
- Operational status: Normal, Disrupted, Secured, Closed, Destroyed, Unknown

The frozen Word schema supplied with the project remains the normative schema source if this convenience summary is ambiguous.


## Artifact / Handout separation (v1.1 extension)

- **Artifact** records describe evidence as an operational object: custody, access, discovery, significance, and relationships.
- **Handout** records contain the complete player-facing document or facsimile content.
- Artifact references use the `A-##` namespace. Handout references use the `H-##` namespace.
- A Handout may be rendered independently without GM material. Its `Player Version` is canonical in-world content.
- Publishers may include `GM Annotation` only in Handler-facing editions.


## Handler Tool extension (v1.1)

- **Handler Tool** records are GM-facing play aids and never exist as documents in the game world.
- Handler Tool references use the `HT-##` namespace.
- Handler Tools may reorganize, summarize, or annotate canonical Source Edition content for use during play.
- Handler Tools must not introduce facts unsupported by their listed canonical source objects.
- Publishers must exclude Handler Tools from player-facing evidence packets.
