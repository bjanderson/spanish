## Interface

- Single, standalone html file containing all HTML, CSS, and JavaScript
- Dark mode styling with blue/green primary/accent color scheme

## Data

- Data saved as separate .json file (spanish-practice.json)
- Automatically load data from spanish-practice.json when the app starts
- data will contain an array of `groups`
- Each `group` will contain a `name` field and an array of `entry` objects
- Each `entry` object will have an `english` field and a `spanish` field
- Provide a button to save data to spanish-practice.json file via download
- Provide a button to load data from local .json file
- Allow user to add data by importing more data files; accumulate data so it can all be saved to the same file
- Do not load data if it is not in the correct format; show an error message; allow the user to dismiss the error message
- Do not add duplicate entries to the same group. All group entries should be unique
- Sort groups by name

## Features

- Present a given text - either in English or Spanish - and let the user enter the translation for that text into a textarea input
- Allow the user to select which language they want the given text to be presented in. Default: English
- Check translated text entered by user against known correct text
- Require translated text to have the correct spelling and accent marks
- Only require correct capitalization and punctuation if the text is a complete sentence
- Do not include any text in parenthesis as part of the translation verification
- Show user the correct text if the entered translated text is incorrect
- Show user a "Correct" message if the entered translated text is correct, and automatically go to the next entry after 3 seconds
- Cycle through all entries in the group and keep cycling as long as the user has incorrect responses. Remove any correct answers from the cycle, but not from the saved .json data
- Allow user to add, edit, and delete groups
- Allow user to select which group to show entries from
- Give user the ability to add, edit, or delete entries within each group
- Give user the ability to move entries to different groups
- Give user the ability to clear the currently loaded data and start fresh
