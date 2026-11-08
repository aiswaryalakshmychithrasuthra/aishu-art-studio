# Project case study — Aishu Art Studio

## Problem

Creative ideas and reference images can become fragmented among the desktop, phone, art folders and social-media posting plans. The aim was a consistent personal workspace that looks like the artist's own sketchbook instead of a generic productivity app.

## Design direction

Warm paper backgrounds; wine/burgundy accents; dark-green actions; oversized editorial serif headings; signature-style logo; portrait collages, pencil drawings and artist photography.

## Cross-platform decisions

- Desktop: preserve the rich home composition and multi-column Art Kitchen.
- Mobile: use a compact fixed navigation bar, responsive cards and a local-first journal.
- Sync: treat local saves, LAN access and Google Drive transfer as distinct features. Do not claim uninterrupted three-way cloud sync before it is verified.

## Testing evidence

1. Windows + Android: Android successfully opened, received a desktop Art Kitchen idea with a reference thumbnail, and displayed a planner entry.
2. Android → Windows: a phone-created test idea appeared on the Windows Art Kitchen list.
3. macOS: native `.app` bundle was built and opened; macOS menu bar displayed Aishu Art Studio.
4. macOS Google Drive folder was linked through the desktop UI.

## Current challenges

- Verify Google Drive Desktop Sync with both desktop devices in real time.
- Complete transfer of all reference/progress media (not just metadata).
- Confirm offline edit → later reconnect → deduplicated merge.
- Improve Android date formatting, sticky-header overlap and long-form editing.
- Audit account-specific configuration and prepare a distributable build.

## Portfolio framing

Role: Creative direction, UX/product design, asset direction, testing, and AI-assisted technical implementation. Avoid claiming that every line of source code was independently handwritten.
