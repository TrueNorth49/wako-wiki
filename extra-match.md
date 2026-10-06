# Extra match

Lucas stated this path on 4 Oct 2026, after matches had already started.

Steps 12 to 23 (the draw and the draw record) were tested on a local copy of the Berner Cup 2026 database with SET 12.2.0 build 3 on 6 Oct 2026. The whole path was run on that copy.

Do this on a new _copy category. Do not generate or save draw records for categories that already have results.

The "Categories: 1" check in step 21 is what keeps the other categories safe.

## A. Copy the category

1. In the Main Tree Menu, right-click "Categories of this event" and choose "Categories of this event".

![Categories of this event](img/extra-match/01-categories-menu.png)

2. An "Attention!" box says: use the same age-limit for registration mode "YEAR OF EVENT" as for "DAY OF EVENT". The conversion and check is made by the system. This is information only. Click OK.

![Attention, OK](img/extra-match/02-attention-ok.png)

3. Highlight the source category row. In the test this was "00 NEWCOMER 02 LC 1129 S M -63 kg". Tip: the Categories window has no entry count column. Check in Move entries first that the source category has athletes, because the Take from list there only shows categories that have entries.

![Source category row](img/extra-match/03-source-row.png)

4. Click "Copy data". The Category Manager opens with the name ending in _copy. Click "save".

![Copy data](img/extra-match/04a-copy-data.png)

![Category Manager, save](img/extra-match/04b-save.png)

5. "Attention! Do you want to use the new category for this event?" Click Yes.

![Use the new category, Yes](img/extra-match/05-use-new-category.png)

## B. Copy the two athletes

6. Right-click "Individual / Team Entries" and choose "Move entries".

![Move entries](img/extra-match/06-move-entries-menu.png)

7. Open the "Take from" dropdown and pick the source category. The athletes in it are listed below.

![Take from](img/extra-match/07-take-from.png)

8. Open the "Move to" dropdown and pick the _copy category. If it is missing, close Move entries and open it again.

![Move to](img/extra-match/08-move-to.png)

9. Check "Copy entries (keep entries in old category)". This keeps the athletes in the old category and also puts them in the new one.

![Copy entries](img/extra-match/09-copy-entries.png)

10. Click the first athlete, then Shift-click the second. In the test these were Doka Anton and Sarikabadayi Ada.

![Two athletes selected](img/extra-match/10-select-athletes.png)

11. Click "Move". "Attention! Do you really want to move the competitors?" Click Yes. The athletes now appear in both categories.

![Move](img/extra-match/11a-move.png)

![Move the competitors, Yes](img/extra-match/11b-move-yes.png)

## C. Draw for the new category only

12. Right-click "Draw" in the tree and choose "Generate draws". This is the single-category item. Do not use "Generate all draws", "Generate all individual draws" or "Generate draws by selection".

![Generate draws](img/extra-match/12-generate-draws-menu.png)

13. In the Draw window, open "Individual categories" and pick the _copy category.

![Individual categories](img/extra-match/13-individual-category.png)

14. Click "Generate draws". A window titled "Generate all draws" (Club / Nation display options) opens. It is SET's shared options screen and only runs for the selected category. Leave the defaults and click Next.

![Generate draws button](img/extra-match/14a-generate-draws.png)

![Generate all draws, Next](img/extra-match/14b-next.png)

15. "Attention! Process finished!" Click OK. The draw shows one Final with the two athletes.

![Process finished](img/extra-match/15a-process-finished.png)

![One Final](img/extra-match/15b-draw-final.png)

16. In the draw window, open the File menu and click Save.

![File, Save](img/extra-match/16-save-draw.png)

17. Click Close on the Draw window.

![Close](img/extra-match/17-close-draw.png)

## D. Draw record for the new category only

18. Right-click "Draw record" in the tree and choose "Save draws as draw records by selection". The window "Save all draws as draw records" opens.

![Save draws as draw records by selection](img/extra-match/18-draw-record-menu.png)

19. Click only the _copy category's row. Rows are highlighted, there are no checkboxes. Do not use "Select all" or "Select draws not saved as draw records".

![Copy category row](img/extra-match/19-select-copy-row.png)

20. If OK is not visible, maximize the window. Click OK.

![Maximize](img/extra-match/20a-maximize.png)

![OK](img/extra-match/20b-ok.png)

21. "Attention! Do you really want to save all draws as draw records? -> Categories: 1". Check that it says Categories: 1. If it shows any other number, click No. Click Yes. Then "Process finished!" appears. Click OK.

![Categories: 1, Yes](img/extra-match/21a-categories-1-yes.png)

![Process finished, OK](img/extra-match/21b-process-finished-ok.png)

22. Right-click "Draw record" and choose Refresh. The count goes up by 1 (77 to 78 in the test).

![Refresh](img/extra-match/22-refresh.png)

23. Under Draw record, double-click the _copy category, then double-click "Pool 1 / 1". The tree cuts the name off, so the _copy entry is the second "00 NEWCOMER 02 LC 1129 S M" line, right after the source category. The draw record opens with the match.

![Pool 1 / 1](img/extra-match/23a-open-pool.png)

![Draw record](img/extra-match/23b-draw-record.png)
