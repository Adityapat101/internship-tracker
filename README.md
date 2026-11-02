# Internship Tracker

A Java terminal program to keep my internship applications and important dates in one place.

So far, only the setup is done. The program prints a welcome message.

## First version

- Add an internship with the company and role.
- View the list of internships.
- Update application statuses, notes, and follow-up dates.
- Show deadlines and follow-ups from soonest to latest.
- Save the list to a file and load it next time.

## Later

- Search by company or role and filter by status.
- Export to CSV.
- Add desktop or email reminders.
- Make a simple graphical interface.

## Tools

- Java 21 or newer.
- Java's built-in tools: `Scanner`, `ArrayList`, `LocalDate`, `DateTimeFormatter`, `Comparator`, `Files`, and `Path`.
- VS Code, Git, and GitHub. No extra libraries or API needed.

## Run it

From the project folder:

```sh
mkdir -p out
javac -d out src/*.java
java -cp out Main
```

For now, it should print `Internship Tracker` and `Work in progress.`, then exit.

## Notes

- [Design](docs/design.md)
- [Feature matrix](docs/matrix.md)
- [Build plan](docs/plan.md)
- [Diagram draft](docs/diagram.png) / [draw.io source](docs/diagram.drawio)

The program starts in `src/Main.java`. I plan to keep entries in an `ArrayList` and use a separate class to save and load them. Personal records will go in `data/`, which is ignored by Git. I'll add tests as I build the features.
