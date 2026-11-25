# PIONEER PSI December Run 2026 – Shift Schedule

Static website (GitHub Pages, served from `docs/`) showing the control-room shift schedule
with day, week and full-run views, the on-call experts, the daily satellite room and the
daily meeting details.

## Updating

The page is generated; do not edit `docs/index.html` by hand.

1. Update the schedule workbook (`PSI_Dec2026_Shift_Schedule_v2.xlsx`).
2. Regenerate: `python build_site.py` (in the folder with the workbook and `scheduler_v2.py`).
   Meeting room and Zoom link are set at the top of `build_site.py`.
3. Publish: `git add -A && git commit -m "Update schedule" && git push`.

## GitHub Pages

Settings → Pages → Source: *Deploy from a branch*, Branch `main`, folder `/docs`.
