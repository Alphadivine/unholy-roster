# Changelog

## 2026-10 — "Perma Killed" status
- Added a **Perma Killed** status for members whose character has been permanently killed (PK'd). Shows a distinct dark-red badge, groups into the **Out** section, and auto-logs "Character perma killed (PK)" to the member's history.
- Available in the member edit form and as an off-list reason in **Import & compare** (Keep / On Leave / Bled out / Perma killed / Left).

## 2026-10 — Seasons + Import/compare
- **Seasons:** each member is tagged to a season; a **Season** dropdown switches between the current season and archived ones; **+ Start new season** (edit mode) archives the current season and starts the next one empty. Requires a new `season` column + `settings` table (Setup guide Step 2e).
- **Import & compare** (edit mode): paste a list of name + stream link, compare to the current season's active roster — add the new people in a click, and for anyone missing from the list choose **Keep / On Leave / Bled out / Left** (auto-logged to their history).
- Discord **Export** now reflects the selected season.

## 2026-09 — Gallery downloads + Multiview
- Gallery photos are downloadable by anyone (tile button + lightbox download).
- Added a **Multiview** button linking to the Unholy Multiview app.

## 2026-09 — Photo gallery
- Added a **📸 Gallery** tab: editors upload photos (auto-compressed to ~1920px), everyone views in a lightbox. Editors-only posting; one-time storage bucket.

## 2026-09 — Core build
- Roster, editable ranks, statuses, automatic Twitch live detection, self-logging history, profile photos with framing, Discord export, hero team photo, white Oswald theme, Supabase backend with shared-password editing.
