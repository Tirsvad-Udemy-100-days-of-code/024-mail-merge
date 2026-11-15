**English** · [Dansk](Home-da) · [Bahasa Melayu](Home-ms)

# Mail Merge

A small script that writes one personalised letter per guest from a template and a list of names.

## What is it?

Day 24 of the Udemy course *100 Days of Code: The Complete Python Pro Bootcamp*. `main.py` reads the guest names from `Input/Names/invited_names.txt`, replaces the `[name]` placeholder in `Input/Letters/starting_letter.txt` with each name and writes one letter per guest to `Output/ReadyToSend/`. It has no tests and no dependencies.

## What the exercise teaches

- Reading a file line by line with `readlines()` and reading a whole file with `read()`
- Removing the trailing newline of each name with `strip()`
- Replacing a placeholder in a template with `replace()`
- Writing one output file per name with `open(..., "w")`

## What it does

- Reads the guest names, one per line, from `Input/Names/invited_names.txt`
- Replaces `[name]` in the letter template `Input/Letters/starting_letter.txt` with each name
- Writes one letter per guest to `Output/ReadyToSend/letter_for_<name>.txt`

## Next

- [Getting Started](Getting-Started)
- [Project Documents](Project-Documents)
