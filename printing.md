# Printing and publishing the match list

Source: process document added 3 Oct 2026. The menu paths on this page were checked on SET 12.2.0 build 3 on 6 Oct 2026.

## Set DTM to List

Open Panels, then "SET DTM". In the "Show / Prin..." row, choose "List". The other two choices are "Portrait" and "Landscape". If "List" is not visible, widen the SET DTM panel by dragging its left edge.

![Panels, SET DTM](img/printing/01a-panels-set-dtm.png)

![SET DTM, Show / Prin... set to List](img/printing/01b-set-dtm-list.png)

The panel also has "Show / Print / Save as... by selection", "Timetable for clubs", the "All draws" and "All draw records" items, "All point tables (DTM)", "Match List", the checkboxes "No page break", "Hide time" and "Override match numbers (Match List, DTM Monitor)", and the Session Matchlist items.

## Match List

You can print via "Match List" in the SET DTM panel. The process document called it "Match list (DTM)". It opens "Please select an item!" with one entry per day and ring, for example "2026-10-04 - Ring 1" to "2026-10-04 - Ring 5". Pick one and click "OK".

![Match List, Please select an item!](img/printing/02-match-list.png)

## Session Matchlist

The cleaner way, once the word Session is in the timetable: print via "Session Matchlist". Select the areas and days. Every session that contains the word Session is offered. Pick the session and print it.

On the local test, "Session Matchlist" opened "Please select an item!" with entries such as "2026-10-04 - Ring 1 - Session start" to "2026-10-04 - Ring 5 - Session start", an "Is Update" checkbox and "OK". The SET DTM panel also has "Session Matchlist as CSV", "Session Matchlist (Generic)", "Session Matchlist (Club)" and "Session Matchlist - TV Names".

![Session Matchlist, Please select an item!](img/printing/03-session-matchlist.png)

## Upload to Sportdata

Save that same document as a PDF and upload it to the event page in Sportdata. Description as appropriate, type Event information. If you upload a new one, remove the previous file. Number them.

To save as a PDF, open Export in the Print Preview window, then Save As PDF... (Ctrl+S). The same menu has Save as text file..., Export to RTF..., CSV, HTML and Excel.

![Print Preview, Export, Save As PDF...](img/printing/05a-export-save-as-pdf.png)

A window titled "Saving Report into a PDF-File ..." opens. Type a Filename or use Select File. OK stays greyed out until a filename is set, and the window says "Please specify a filename for the pdf file." Then click OK.

![Saving Report into a PDF-File, Filename and Select File](img/printing/05b-pdf-filename.png)

On SET 12.2.0 build 3 (local test, 6 Oct 2026): this was the Match List preview from the Match Caller panel. Cancel was clicked, so no PDF was saved.

The upload was not tested on 6 Oct 2026, because it goes online.

## If something changes

1. Go back to match calling. Open Panels, then "Match Order / Lists / Caller". The side panel is headed "Match Caller". Click the big Match Caller icon. The "Match calling" window opens.

![Panels, Match Order / Lists / Caller](img/printing/04a-panels-match-order-lists-caller.png)

![Match Caller icon](img/printing/04b-match-caller.png)

2. Select the match. The status line shows "1 matches selected".

3. Click "Delete matches". It is in the "Main Options" bar at the bottom of "Match calling". The local test did not click it.

![Match calling, Delete matches and Edit number](img/printing/04c-match-calling-delete-edit-number.png)

4. Go back to the draw and fix it.

In the tree, under Draw, right-click the category, then click Open draw / Edit. To change the order, click Edit, then Manually changes. The full steps are in [Match the ring plan](ring.md?id=match-the-ring-plan).

![Draw, Open draw / Edit](img/ring/03a-open-draw-edit.png)

![Edit, Manually changes](img/ring/03b-manually-changes.png)

5. Return to this list and insert it again at the right number. Shift the others.

"Edit number" is in the same "Main Options" bar, with "Show in tree", "Reset match", "Draw record", "Delete missing n..." (cut off on screen) and "Refresh / Reset". "Assign number" and "Unset number" are under the draw record list on the left. Re-inserting at a number was not tested.

On SET 12.2.0 build 3 (local test, 6 Oct 2026): match #1 was selected ("1 matches selected"), then Edit number.

![Main Options, Edit number](img/printing/06a-edit-number.png)

A box titled "Edit number: #1 07 K1 390 YJ M -57 kg" opened, with one text field, OK and Cancel. Cancel was clicked, so the number did not change.

![Edit number box with its text field](img/printing/06b-edit-number-dialog.png)

"Assign number" and "Unset number" are at the bottom of the Draw record/Point table list. Both were only hovered.

![Assign number and Unset number](img/printing/06c-assign-unset-number.png)
