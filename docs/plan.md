# Build plan

Each step is planned as one Git commit. Step 1 is done; the rest still need to be built. I'll check input as I go, then do another pass in step 8.

1. **Set up the project.** Add the Java starter, GitHub repo, README, and planning notes. Compile and run the starter.
2. **Make the `Internship` class.** Add the ID, company, role, status, link, dates, and notes. Put a few made-up entries in an `ArrayList` and display them.
3. **Add the menu.** Use `Scanner` to add internships, view the list, and exit. Try several entries and an invalid menu choice.
4. **Update entries.** Choose an internship by ID and change its status, notes, or follow-up date. Check that the right entry changes and that a missing ID is handled.
5. **Save the list.** Write all fields to a file in `data/`. Check the file with a few entries, including blank optional fields.
6. **Load the list.** Read the file when the program starts and keep the same IDs. Try restarting, an empty file, and a missing file.
7. **Show upcoming dates.** List deadlines and follow-ups from soonest to latest. Try past dates, matching dates, blank dates, and an empty list.
8. **Handle errors.** Check invalid numbers, missing required fields, impossible dates, and unreadable files. Make sure a failed load doesn't overwrite saved information.
9. **Try the whole program.** Add, update, save, close, reopen, and check dates. Write down the results and finish the README with usage examples.
