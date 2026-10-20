# Changelog

## 2026-10 — Smarter import: first-name matching + stream-change detection
- **Import & compare** now matches on **first name** (the Discord list usually only has a character's first name), so "Jesse" on the list matches "Jesse James" in the roster instead of showing as both new and missing. Twitch login still takes priority when present.
- New **🔗 Stream changed** section: for people already in the roster, if their stream link on the pasted list differs from what's stored, it's flagged with old → new and you can update the saved link in a click (keeps their other platforms; auto-logs to history).

## 2026-10 — Fix: "Start new season" button hidden on single-season setups
- The Season bar (and its **+ Start new season** button) was hidden whenever only Season 1 existed — exactly when you need it. It now shows in **edit mode** regardless of season count, so editors can always start the next season. Viewers still only see the bar once more than one season exists.

## 2026-10 — Per-member season control
- The member edit form now has a **Season** dropdown (shown once more than one season exists) to **move** a person to a different season.
- Added a **⇧ Carry over to current season** button that **copies** a member into the current season while leaving their archived record intact — for core members who continue into the new season.
- Both auto-log to the member's history ("Carried over from Season N").

## 2026-10 — Season-aware gallery
- The **📸 Gallery** now follows the active season: existing photos become Season 1, new uploads are tagged to the season you're viewing, and switching seasons filters the photos to match.
- Empty seasons show a hint pointing to photos in other seasons. Requires a `season` column on the `gallery` table (Setup guide Step 2e).

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
