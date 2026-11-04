# Weekly Timesheet

A lightweight, browser-based timesheet for tracking working hours, lunch breaks, weekly notes, holidays, and Excel exports.

**Live app:** [timesheet-delta-seven.vercel.app](https://timesheet-delta-seven.vercel.app/)

## Quick start

1. Open the live app.
2. Use the **My standard day** section to set your usual work and lunch times.
3. For an existing week, select **Apply to this week** to use those times on weekdays.
4. Adjust individual days directly, or use **↺ Default** beside a day to reset it to the standard schedule.
5. Enter your weekly work notes and choose **Download this week** when ready.

Edits save automatically in the current browser.

## Default working pattern

| Field | Value |
| --- | --- |
| Time in | 9:00 AM |
| Lunch starts | 1:15 PM |
| Lunch ends | 1:45 PM |
| Time out | 6:00 PM |
| Default days | Monday–Friday |

That is **8.5 worked hours per standard weekday**, or **42.5 hours across five weekdays** after the 30-minute lunch deduction. The app currently calculates regular hours up to 40 per week and displays the remainder as overtime.

## Features

- Navigate between weeks and jump back to the current week.
- Save a standard schedule for new weekdays.
- Apply defaults to the current week or reset a single day.
- Mark days off, including holidays.
- Select multiple days and copy or adjust their times.
- Bulk-fill an entire week, month, or date range.
- Add weekly notes and export one week or all saved weeks to `.xlsx`.
- Import saved timesheet data from Excel.

## Data and privacy

**This app uses browser `localStorage`, not an online account or synchronized database.** Data stays in the browser and device where it was entered; clearing site storage may erase saved weeks. Keep Excel backups and do not expect entries to appear automatically on a different browser or computer.

## Repository layout

- `index.html` — the current production application
- `timesheet.html` — an older standalone version retained for reference

The live application is deployed through Vercel. Since it is a static HTML/JavaScript app, you can also open `index.html` locally in a modern browser, though downloading or importing spreadsheets requires the external XLSX library to load.

## Development

No build step is required. Changes to `index.html` should be checked for working time controls, accurate calculations, navigation/autosave, and Excel export behavior before deploying.
