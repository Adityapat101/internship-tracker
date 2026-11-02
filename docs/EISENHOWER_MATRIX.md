# Eisenhower Matrix

Project: Java Command-Line Internship Tracker

The **Do** quadrant defines the MVP. Every feature considered for this project is assigned below. Library tasks in **Delegate** support the MVP features; they describe code I can reuse from Java instead of building utility functions from scratch.

| | Urgent | Not Urgent |
| --- | --- | --- |
| **Important** | **Do — MVP**<br>1. Add an opportunity with company, role, status, and optional dates.<br>2. List saved opportunities and their details.<br>3. Update an opportunity's status, notes, and follow-up date.<br>4. Save records locally and load them when the app starts.<br>5. Show upcoming deadlines and follow-ups in date order. | **Schedule — V2.0+**<br>1. Search by company or role and filter by status.<br>2. Export records to a spreadsheet-friendly CSV file.<br>3. Add desktop or email reminders.<br>4. Build a simple graphical interface. |
| **Not Important** | **Delegate — Use a Library**<br>1. Use `LocalDate` and `DateTimeFormatter` for date parsing and comparisons.<br>2. Use `Files` and `Path` for reading and writing files.<br>3. Use `Comparator` and Java's built-in list sorting for date order. | **Delete — Cut It**<br>1. Automatically apply to jobs or send outreach emails.<br>2. Generate cover letters or resumes with AI.<br>3. Add a social feed, profiles, or messaging between users.<br>4. Add accounts and cloud synchronization. |

## Why This Is the MVP

These features cover the full basic workflow: enter an opportunity, track progress, save it, return later, and check the next important dates. The later features can improve convenience, but the app will already solve the original organization problem without them.
