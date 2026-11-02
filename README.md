# Internship Tracker

A small Java project to keep track of internship applications, deadlines, and when to follow up.

Right now it just prints a welcome message. I still need to build the actual tracking features.

## First version (MVP)

- Add internships with the company, role, and application link.
- Update the status and keep notes about each application.
- Show upcoming deadlines and follow-up dates.
- Save everything to a file and load it the next time I open the program.

## Later on

- Search by company or role and filter by application status.
- Export the list to a CSV file.
- Add desktop or email reminders.
- Try making a simple graphical interface.

## Tech stack

- Java 21, with `Scanner` for input and an `ArrayList` for the internship list.
- `LocalDate` and `DateTimeFormatter` for dates, and `Comparator` for sorting.
- `Files` and `Path` for saving and loading a local text file.
- VS Code, the terminal, Git, and GitHub.

## How to run it

You need JDK 21 or newer. There are no extra libraries to install. From the project folder, run:

```sh
mkdir -p out
javac -d out src/*.java
java -cp out Main
```

For now, it should print this and exit:

```text
Internship Tracker
Work in progress.
```

## Project files

- `src/Main.java` is where the program starts.
- [Design](docs/DESIGN.md) explains the idea and tools.
- [Eisenhower Matrix](docs/EISENHOWER_MATRIX.md) lists what goes in the first version and what can wait.
- [Build plan](docs/MILESTONES.md) has the steps I plan to follow.

The system diagram and its editable source still need to be added.

The plan is to keep `Internship` objects in an `ArrayList` and use a separate class for saving and loading files. Personal records will go in `data/`, which is ignored by Git. I'll use made-up records for examples and tests.

The compile-and-run check above is the only check so far. I'll add tests as I build the features.
