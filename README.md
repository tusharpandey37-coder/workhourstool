# Weekly Office Hours Tracker

A static GitHub Pages tool for checking weekly attendance against the 42 hours 30 minutes requirement.

## Deploy on GitHub Pages
1. Create a GitHub repository.
2. Upload `index.html`, `holidays.json`, and this `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
5. Wait for the Pages URL to appear.

## How it works
- Upload the attendance CSV exported by the attendance system.
- Choose any date in the week; the tool displays that Monday–Friday week.
- The export's date field and final `HH:MM:SS` duration field are read locally in your browser.
- Weekends are not shown because they are always excluded.
- Maharashtra Central Government office holidays from the supplied 2026 circular are excluded automatically.
- Each included weekday adds 8 hours 30 minutes to the weekly target. A normal five-day week therefore requires 42:30; one unchecked leave day makes it 34:00.
- Untick a weekday if you took leave. The requirement is reduced by 8:30 for that day, while any recorded attendance duration remains included in worked hours.
- No CSV data is sent to a server.

## Holiday updates
The current holiday list is also documented in `holidays.json`. The list in `index.html` is embedded so the app works as a simple static site; update both files when adding another year.
