# Session Logger

A tool a researcher can keep open during a usability test to time each task and record whether the participant succeeded and how many errors they made.


## Why I made this
When you run a moderated session you are watching the participant, taking notes, and trying to keep track of time all at once. I wanted something simple that does the counting so the researcher can pay attention to what the person is doing. It is also the kind of data you would analyze later, so I made it export cleanly.

## What it does
Type a task name and a participant ID, press Start, and a timer runs. During the task you can log errors with one button. When it ends you mark it as a success or a fail. Every task goes into a table, and the page shows the success rate, average time, and average errors. Sessions are saved in the browser, and you can export everything to CSV.

## What I did
- Built the timer with `requestAnimationFrame` so the display stays smooth.
- Stored sessions in `localStorage` so a refresh does not lose the data.
- Escaped user text before putting it in the page, and quoted it properly in the CSV, so task names with commas or quotes do not break anything.
- Disabled buttons that should not be clickable at a given moment, so you cannot log an error when no task is running.

## Skills used
JavaScript, DOM, `localStorage`, CSV export, usability testing metrics (task success, time on task, error rate), HTML, CSS, accessible form design.

## Roles this project fits
UX Researcher, UX Engineer, Research Assistant, Product Analyst, Front-End Engineer.

## Run it
Open `index.html` in a browser.

## What I would add next
Notes with timestamps for each task, and a chart of time on task by participant.
