# Unholy Roster — HeadlinerRP

Live gang roster & stream tracker for the Unholy crew on HeadlinerRP. One self-contained web page backed by Supabase (free tier).

## Features
- Roster grouped by rank (custom, editable ranks with insignia), plus **On Leave** and **Out** (bled out / perma killed / removed) sections
- Member **statuses**: Active, On Leave, Inactive, Bleedout, **Perma Killed** (PK'd), Removed — status changes auto-log to history
- Automatic **Twitch live detection** + "Live now" spotlight strip
- Click-through **profiles** with history timeline and stream links (Twitch / YouTube / Kick / TikTok)
- **Profile photos** with framing (position / zoom / fill) and banner cover cards
- **Photo gallery** — editors post (auto-compressed), everyone views in a lightbox and can download; season-aware
- **Seasons** — archive past seasons, start new ones empty; roster *and* gallery filter by season; move or carry members between seasons
- **Discord export** (name + Twitch link) and **Import / compare** (reconcile against a pasted list)
- Hero team photo, Multiview button, shared-password editing (Supabase RLS)

## Setup
See `../Docs/Setup guide.md`. Needs a free Supabase project; keys go in the `CONFIG` block near the bottom of `index.html`.

## Hosting
Static site — host `index.html` on GitHub Pages (repo must be public; only the publishable key is in the file) or Netlify.

Last updated: 2026-10-20
