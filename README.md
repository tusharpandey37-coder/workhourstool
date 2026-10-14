# Weekly Hours Tracker

Static GitHub Pages tool for checking weekly attendance against the 42 hours 30 minutes requirement.

## Publish
Upload `index.html`, `holidays.json`, and `README.md` to the repository root. In Settings → Pages, choose Deploy from a branch, `main`, and `/(root)`.

## Notes
- The current Monday–Friday week is selected automatically.
- Up to two monthly CSV files can be selected together.
- CSV attendance duration is read in HH:MM:SS format.
- A CSV attendance record locks the leave checkbox for that day.
- Register day credits the daily benchmark of 8 hours 30 minutes.
- The exit planner defaults to 09:00 and 17:30.
- Train results are indicative sample timetable entries, not live running data. Check the linked eRail timetable before travelling.
- Attendance data is processed locally in the browser.
