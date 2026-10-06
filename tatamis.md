# Tatamis

Source: process document added 3 Oct 2026. The menu paths on this page were checked on SET 12.2.0 build 3 on 6 Oct 2026.

Ring draws, draw records, and match calling: [Ring](ring.md).

Copy a category for an extra match after matches have started: [Extra match](extra-match.md).

## Draws

In the Main Tree Menu, right-click "Draw", then "Generate draws by selection", and select the tatami categories.

![Draw, Generate draws by selection](img/tatamis/01a-generate-draws-by-selection.png)

The window is titled "Generate draws". At the bottom are "Select draws not done", "Select all", "OK" and "Refresh".

![Generate draws](img/tatamis/01b-generate-draws-window.png)

If draws already exist, use "Select draws not done" so you do not overwrite or regenerate them.

On SET 12.2.0 build 3 (local test, 6 Oct 2026): every draw on the copy already existed, so "Select draws not done" highlighted no rows. No tatami rows were selected in the test.

![Select draws not done, no rows highlighted](img/tatamis/01c-select-draws-not-done.png)

## Draw records

Right-click "Draw record", then "Save draws as draw records by selection". Select the tatami categories.

![Draw record, Save draws as draw records by selection](img/tatamis/02a-save-draws-by-selection.png)

The window is titled "Save all draws as draw records". At the bottom are "Select draws not saved as draw records" and "Select all". The OK button is hidden until you maximize the window.

![Save all draws as draw records](img/tatamis/02b-save-draws-window.png)

Also use "Select draws not saved as draw records", so existing records are not overwritten.

## Print

Venue note (Lucas, 4 Oct 2026, SET 12.2.0 build 2): List, then All draw records as PDF. Select the areas you want for that day.

Not found on SET 12.2.0 build 3 (local test, 6 Oct 2026). Found instead: there is no "List" or "Print" submenu. "All draw records as PDF" is directly in the right-click menu on "Draw record".

![Draw record, All draw records as PDF](img/tatamis/03a-all-draw-records-pdf.png)

It opens "Club / Nation display options".

![Club / Nation display options, Next](img/tatamis/03b-club-nation-options.png)

Next goes straight to a "Save in directory ..." dialog. There is no ring or day choice.

![Save in directory, folder blurred](img/tatamis/03c-save-in-directory.png)

The folder path is blurred in the screenshot.

To print only certain rings or days, use SET DTM below.

## Big overview

For the big overview, use "Show / Print / Save as... by selection" (the second option).

Open Panels, then "SET DTM".

![Panels, SET DTM](img/tatamis/04a-panels-set-dtm.png)

Click "Show / Print / Save as... by selection". A "Please select an item!" window lists one entry per day and ring, for example "2026-10-04 - Ring 1" to "2026-10-04 - Ring 5". Pick the entry and click "OK".

![Show / Print / Save as... by selection](img/tatamis/04b-show-print-save-as-by-selection.png)

That makes a short list per area, in time order, so people can see the plan.

On SET 12.2.0 build 3 (local test, 6 Oct 2026): the preview below was opened from the Match Caller side panel (Panels, then Match Order / Lists / Caller), with "Show / Print / Save as...". The SET DTM "by selection" list itself was not opened. "Automatically hide finished m..." (cut off) was ticked in the same panel.

![Match Caller, Show / Print / Save as... and Automatically hide finished m...](img/tatamis/05a-match-caller-show-print.png)

It asked "Please select an item!" with 2026-10-04 - Ring 1 to Ring 5. Ring 1 was picked, then OK.

![Please select an item!, Ring 1, OK](img/tatamis/05b-select-ring-1.png)

A Print Preview titled Match List opened, with the columns #, Category, Red, Blue, Round, Ring, Type, Time and Day. It had no rows, because the matches on the local copy are finished and finished matches were hidden.

![Print Preview, Match List with no rows](img/tatamis/05c-match-list-preview.png)
