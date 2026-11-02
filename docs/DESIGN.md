# Internship Tracker Design

## 1.1: The Problem I Want to Solve

When I look for internships, I end up with information in job websites, emails, and spreadsheets. It gets hard to remember where I applied, which deadlines are coming up, and who I need to follow up with. Since I'm applying for internships myself, I want one place to keep this information.

## 1.2: My Idea

I'm going to build a Java program that runs in the terminal and lets me add internships, update their statuses, and check upcoming dates. It will save the list to a local file so I don't lose it when I close the program.

## 2.1: MVP

For the first version, I want to add an internship, view it, change its status, and save it. I should be able to close the program, open it again, and see the same information and upcoming dates. The rest of the features are sorted in [the Eisenhower Matrix](EISENHOWER_MATRIX.md).

## 2.2: Languages, Libraries, Commands, and Tools

- Java for the program. This gives me practice with classes, methods, loops, and user input.
- An `Internship` class to keep the details of one internship together.
- `ArrayList<Internship>` to store the list while the program is running.
- `Scanner` to read menu choices and other input. I'll read whole lines so invalid choices are easier to handle.
- `LocalDate` and `DateTimeFormatter` to read and compare dates, entered as `yyyy-MM-dd`.
- `Files` and `Path` to read and write the saved file.
- `Comparator` to sort deadlines instead of writing a sorting algorithm myself.
- VS Code to edit the code and documents.
- The terminal, `javac`, and `java` to compile and run the program.
- Git and GitHub to save my progress after each step.
- Markdown for the README and planning documents.

I'll enter the internship information myself. This version won't need an API or database, and all the Java tools above are built in.

## How I plan to organize it

Each internship will have an ID number, company, role, and status. The link, deadline, follow-up date, and notes can be left blank. The statuses will be `Interested`, `Applied`, `Interviewing`, `Offer`, and `Rejected`.

The menu will have options to add, list, update, view upcoming dates, save, and exit. The program will load the saved list when it starts. I'll use the ID number to select an internship, and that number should stay the same after saving and loading.

I plan to save the list in `data/internships.tsv`, with one internship per line and tabs between its fields. I'll reject tabs and line breaks inside text fields so they don't break the format. A blank date will mean there isn't one. The `data/` folder will stay out of Git because it can contain personal application details.

I'll check input as I add each feature. The program should explain invalid choices and dates, work on the first run without a saved file, and tell the user if saving fails.

## 2.3: Build Plan

See [the build plan](MILESTONES.md). So far, only step 1 is done.

## 2.4: System Diagram

Not added yet. I still need to draw the diagram in a diagramming tool, embed the exported PNG or JPG here, and add the editable source file to the repo.

## 3.1: GitHub Repository

[Internship Tracker on GitHub](https://github.com/Adityapat101/internship-tracker)
