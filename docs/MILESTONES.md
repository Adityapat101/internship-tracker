# Chunked Build Plan

Each step is planned as one Git commit. Step 1 is done; the rest still need to be built. I'll check input as I go, then do another pass in step 8.

1. **Set up the project and GitHub repo.** Add the Java starter, `.gitignore`, README, and planning documents. Compile and run the starter to check the setup.
2. **Make the `Internship` class.** Give each internship an ID, company, role, status, link, dates, and notes. Put a few made-up entries in an `ArrayList` and check that they display correctly.
3. **Add the menu.** Use `Scanner` so I can add internships, view the list, and exit. Try adding more than one entry and entering an invalid menu choice.
4. **Update applications.** Choose an internship by ID and change its status, notes, or follow-up date. Check that it changes the right entry and handles an ID that doesn't exist.
5. **Save the list.** Write all the fields to a file in `data/`. Check the saved file with a few made-up entries, including ones with blank optional fields.
6. **Load the list.** Read the file when the program starts and keep the same IDs. Check that entries are still there after restarting, and that the program works with an empty or missing file.
7. **Show upcoming dates.** List deadlines and follow-ups from earliest to latest. Try past dates, matching dates, blank dates, and an empty list.
8. **Handle bad input and file errors.** Check invalid numbers, missing required fields, impossible dates, and files that can't be read. Make sure a failed load doesn't lead to overwriting saved information.
9. **Try the whole program and finish the README.** Add an internship, update it, save, close, reopen, and check the upcoming dates. Write down the results and add usage examples to the README.
