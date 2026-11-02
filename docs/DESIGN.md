# Internship Tracker Design

## 1.1: The Problem I Want to Solve

When I look for internships, the information ends up spread across job websites, emails, and spreadsheets. It is easy to forget which companies I have applied to, when applications close, or when I should follow up. I care about this because I am applying for internships myself and want a simpler way to keep track of everything.

## 1.2: My Idea

I will build a Java command-line internship tracker where I can manually add opportunities, update application statuses, and see upcoming deadlines and follow-up dates. It will save records in a local file so I can keep using the same list after closing the program.

## 2.1: MVP

The smallest complete version lets a user add an opportunity, view it, update its status, save it, restart the program, and see the saved opportunity and its upcoming dates. The full feature decisions are in [the Eisenhower Matrix](EISENHOWER_MATRIX.md).

## 2.2: Languages, Libraries, Commands, and Tools

- **Java:** I will use Java for the program because I want to practice classes, methods, loops, and working with user input.
- **An `Internship` class:** Each object will represent one opportunity and keep its details together.
- **`ArrayList<Internship>`:** This will hold the opportunities while the program is running.
- **`Scanner`:** I will use it to read menu choices and details typed into the terminal. Reading whole lines will make it easier to handle invalid menu choices.
- **`LocalDate` and `DateTimeFormatter`:** These built-in Java tools will help parse, check, and compare dates. I will use the format `yyyy-MM-dd`.
- **`Files` and `Path`:** These built-in tools will read and write the local records file.
- **`Comparator`:** This will help sort upcoming deadlines and follow-up dates without writing my own sorting algorithm.
- **VS Code:** I will use it to edit the Java source files and project documents.
- **The terminal, `javac`, and `java`:** I will compile the source code and run the app from the command line.
- **Git and GitHub:** I will save each milestone as a commit and keep a private remote copy of the project.
- **Markdown:** I will keep the README, design document, matrix, and milestone list in the repository so they can be updated with the code.

The MVP will use manual entry and local files. It does not need an API, database server, paid service, or external Java library.

## Planned Data and Flow

Each internship will have a stable numeric ID, company, role, optional application link, application status, optional deadline, optional follow-up date, and optional notes. The first statuses will be `Interested`, `Applied`, `Interviewing`, `Offer`, and `Rejected`.

The menu will let the user add, list, update, view upcoming dates, save, and exit. Records will be loaded at startup. IDs will stay the same after saving and loading, so the user can choose an entry without depending on its current position in the list.

The planned storage file is `data/internships.tsv`, with one record per line and tabs between fields. To keep the first version simple, text fields will reject embedded tabs and line breaks. Blank date fields will mean no date was supplied. The `data/` directory will stay out of Git because it can contain personal application information.

Input checks will be added with each relevant feature. The app should explain invalid choices and dates, handle a missing file on the first run, and report file errors without claiming a save succeeded.

## 2.3: Build Plan

See [the ordered milestone list](MILESTONES.md). Only the setup milestone is complete at this point.
