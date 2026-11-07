# EDEK WWW v2 — CORRECTION REVIEW 2026-11-07 (YouTube Studio AI)

## Source
Owner-provided second AI Studio response in conversation (2026-11-07). This is self-reported Studio AI output, **not an independent YouTube Analytics API response**.

## Facts claimed by AI Studio
- 41 "Film" records in the earlier exported table, now described as *public and non-public*; initial 104 public items (32 films + 72 Shorts) remains a **separate claim**, not a resolved shared population.
- IDs in the 41-row list are claimed to be read directly from YouTube.
- COUNT THE FEW XjevEYJzNMI: 28-day watch time 20:57:54; average view duration 65 seconds; 28-day views 1560; lifetime average viewed 27.28%.
- BILANS C4RHQ9u0Loo: 28-day views 323 and watch time 9:53; initial lifetime views 284 and watch time 8:44.
- Thumbnail asset URLs unavailable within Studio AI interface; earlier user-supplied screenshots establish appearance of some published thumbnails but not video URLs.

## Outstanding QA: do NOT mark resolved
1. **Counts/status**: 41 film records reportedly include nonpublic items while 104 count reportedly covers public only. Plausible that 32 public + 9 other statuses = 41, but this is NOT confirmed without per-video privacyStatus. Don't publish nonpublic items.
2. **COUNT THE FEW arithmetic**: 1560 views × 65 sec = 101400 sec = 28h 10m. Reported 20h57m54s = 75474 sec -> 48.38 seconds/watch if divided by 1560 views. AI explains mismatch as invalid sessions without furnishing the actual metric definitions/filters; unverified and potentially erroneous. Do not calculate projected growth from these mixed metrics.
3. **BILANS chronology**: 323 views in first 28 days exceeds reported 284 lifetime views at later date; same metric and scope cannot have these values. 9h53m (28-day) also exceeds reported lifetime 8h44m. Request two matched period Studio screenshots/exports or use data with ranges explicitly labelled; avoid unverified explanations.
4. User screenshots have counts slightly or markedly different from earlier AI Studio totals; retain as distinct dated observations, not a single canonical count without same read date/scope.
5. Neither report provides measured thumbnail impressions sample sizes; ranking by CTR can overstate small samples.

## Data governance
- **Provisional catalogue**: 41 claimed 11-character video IDs and title/date metadata, pending public status per ID. IDs are candidate linkage keys, NOT independently verified.
- **Verified from owner screenshots**: published thumbnail visual designs, a subset of names and public visibility in the app at screenshot time, not the full metadata.
- **Not suitable for website**: dynamic counts, CTR, watch times, asserted 'TOP 9' selected solely by AI Studio, the 32/41/72 breakdown unless status clarified.
- Approved next task: build **read-only** public catalog and cards around source video IDs, but only after determining privacyStatus = public; use public canonical YouTube URLs/thumbnails where available. Avoid publishing raw Studio analytics.
- Do not change production `main`; existing website v1.3 remains intact.

## Narrow next data request if Studio can export
Return **per-video** `videoId, title, privacyStatus, videoType, publishedAt` for the 41 rows, with date and timezone of export. If numeric analytics needed later, use **matching metric/date ranges** for COUNT THE FEW and BILANS and show exact fields `views, watchTimeHours, averageViewDurationSeconds`. A direct CSV export from YouTube Studio is preferable to another narrative AI summary.
