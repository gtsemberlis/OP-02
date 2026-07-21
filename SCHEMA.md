# OP-02 Source Repository Schema v1.0

**Status:** Normalized after content lock.

Every canonical object contains YAML front matter with: `id`, `title`, `type`, `status`, `content_status`, `operation`, `canonical_path`, and `related_objects`. Scenes additionally declare `primary_location`.

## Stable ID Namespaces

- `SC-##` — Scenes
- `PER-##` — Personnel
- `LOC-##` — Locations
- `A-##` — Artifacts
- `HT-##` — Handler tools

## Canonical Linking

Markdown links in each object's **Canonical Relationships** section are authoritative navigational links. YAML relationship IDs are authoritative machine-readable relationships.

## Content Preservation

Normalization may restructure headings, filenames, metadata, and links. It must not silently omit locked canonical prose.
