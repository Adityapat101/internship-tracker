# Internship Tracker

A first-year Java command-line project for keeping internship opportunities, application statuses, deadlines, and follow-up dates in one place.

## Current progress

Milestone 1 is complete: the repository, runnable Java starter, design document, Eisenhower Matrix, and build plan are set up. The starter currently prints a welcome message. The tracking features below are planned work.

## Planned MVP

- Manually add and view internship opportunities.
- Update application statuses and follow-up information.
- Save records locally and load them after restarting.
- Display upcoming application deadlines and follow-up dates in date order.

No external API or internet connection will be needed to run the MVP.

## Requirements

- JDK 21 or newer, including `java` and `javac`.
- Git for version control.
- A terminal and an editor such as VS Code.

No external Java libraries, package manager, or build tool are required for the starter. Check your Java installation with:

```sh
java -version
javac -version
```

## Build and run

Run these commands from the project folder:

```sh
cd /Users/adipat/Documents/Ideas_ADI/internship-tracker
mkdir -p out
javac -d out src/*.java
java -cp out Main
```

The current output is:

```text
Internship Tracker
Project setup complete. Tracking features are planned for the next milestones.
```

## Check the starter

Compile and run using the commands above. The program should print the two lines shown and exit normally. There is no automated test suite yet because the starter has no tracking behavior. Checks for adding records, updating them, saving, loading, and sorting will be added alongside those features.

## Structure and planned architecture

- `src/Main.java`: current entry point; the command-line menu will start here.
- `docs/DESIGN.md`: problem, solution, planned data model, and technology choices.
- `docs/EISENHOWER_MATRIX.md`: MVP and later feature decisions.
- `docs/MILESTONES.md`: nine ordered steps, each intended to be one meaningful Git commit.

The app will keep `Internship` objects in an `ArrayList`. A small file-storage class will handle local persistence. A `tests/` directory will be added when there is behavior to test. Personal records will go in the ignored `data/` directory; only fictional examples should appear in committed examples or tests.
