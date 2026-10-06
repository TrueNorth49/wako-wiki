# Upload results to SET Online

Source: the Sportdata knowledge base article [Upload draws, timetable & results](https://set.sportdata.org/knowledge-base/upload-draws-timetable-results/) and Lucas's process. The menu paths were checked on SET 12.2.0 build 3 (local test, 6 Oct 2026). The knowledge base screenshots are from SET v11 and are not copied here.

> **Warning:** Clicking "Upload results to SET Online on www.sportdata.org / Kickboxing Events APP" uploads at once. There is no extra step. SET pushes the results online as an XML file and they show on the event page under Results. On SET 12.2.0 build 3 (local test, 6 Oct 2026) the upload lines were only hovered, never clicked. Nothing was uploaded.

## Upload results

1. Click "Panels" in the menu bar.

![Panels](img/upload-online/01-panels-menu.png)

2. Choose "SET Online Kickboxing / Kickboxing Events APP". The panel opens on the right side, headed "SET Online Kickboxing / Kickboxing Events APP". Double-click its title bar to widen it, so the full line texts show. This is also the knowledge base tip. Dragging the left edge did not resize it in the local test.

![Panels, SET Online Kickboxing / Kickboxing Events APP](img/upload-online/02-set-online-kickboxing.png)

On SET 12.2.0 build 3 (local test, 6 Oct 2026) the panel opened docked on the right side, about half the width of the window. Its title bar and left edge are boxed below.

![SET Online Kickboxing panel, title bar and left edge](img/upload-online/07-panel-edge-title.png)

In the same test the left edge was dragged to the left. The panel did not resize. The edge is boxed below.

![SET Online Kickboxing panel docked on the right, left edge not resized by dragging](img/upload-online/07b-panel-docked-drag-no-resize.png)

Double-clicking the title bar maximized the panel to the full width of the window. Double-clicking the title bar again restored it to the docked size.

![SET Online Kickboxing panel maximized after a double-click on its title bar](img/upload-online/07c-panel-maximized-double-click.png)

3. Scroll down the panel to the "Results" section. Its sections from top to bottom are "SET Online Kickboxing / Kickboxing Events APP", "SET Liveblog Synchronizer", "Info and PSS Uploader / Match Schedule", "SET DTM Monitor Live Synchronizer", "Activity Monitor Live Synchronizer", "Match Caller Monitor Live Synchronizer", "Match Caller Area Monitor Live Synchronizer", "SET DTM - Dynamic Time Management", "Draw, Draw record, Point Draw...", "Results", "Download online photo" and "Online Downloads Section". The arrow at the right end of each title opens or closes the section.

On SET 12.2.0 build 3 (local test, 6 Oct 2026), with every section closed except "Online Downloads Section":

![SET Online Kickboxing panel, all sections closed](img/upload-online/08-sections-collapsed.png)

4. Click "Upload results to SET Online on www.sportdata.org / Kickboxing Events APP". Its tooltip reads "Upload results to SET Online on www.sportdata.org". The upload starts at once.

![Results, Upload results to SET Online on www.sportdata.org](img/upload-online/03-upload-results.png)

The local install has these texts for the results upload: "Generating results as XML data", "Processing...Please wait!" and "Process finished!". On a failure it has "Error on uploading the results!". If the upload fails, check the internet connection. (The last sentence is from the knowledge base.) The knowledge base also says to select the "Attention!" option for any necessary alerts. On the local test no window was opened, so this was not seen.

## Upload only some categories

Use "Upload results to SET Online on www.sportdata.org by selection / Kickboxing Events APP" to upload chosen categories only. The selection window was not opened on the local test.

![Results, by selection](img/upload-online/04-upload-results-by-selection.png)

## Remove uploaded results

"Remove uploaded Results" takes the uploaded results off the event page. Its tooltip is misspelled "Remove uplaoded Results" in SET. It was not clicked on the local test.

![Results, Remove uploaded Results](img/upload-online/05-remove-uploaded-results.png)

## Upload draws during the event

Draws, draw records and point draws can be uploaded the same way during the event, once they are final. In the "Draw, Draw record, Point Draw..." section click "Upload draws and records to SET Online on www.sportdata.org / Kickboxing Events APP". Its tooltip reads "Upload draws and records to SET Online on www.sportdata.org". The section also has "Upload draws and records to SET Online on www.sportdata.org by selection / Kickboxing Events APP" and "Remove uploaded Draws, Draw Records and Point Lists". The knowledge base says to select either all draws or by selection, and that a confirmation pop up appears once completed. Not clicked on the local test.

![Draw, Draw record, Point Draw..., Upload draws and records](img/upload-online/06-upload-draws-and-records.png)

On SET 12.2.0 build 3 (local test, 6 Oct 2026) the other two lines were only hovered, never clicked. The "by selection" line has the tooltip "Upload draws and records to SET Online on www.sportdata.org by selection".

![Draw, Draw record, Point Draw..., by selection, tooltip](img/upload-online/12-draws-by-selection-hover.png)

"Remove uploaded Draws, Draw Records and Point Lists" showed no tooltip in the test.

![Draw, Draw record, Point Draw..., Remove uploaded Draws, Draw Records and Point Lists](img/upload-online/13-draws-remove-hover.png)

## Timetable

The "SET DTM - Dynamic Time Management" section has "Upload timetable to SET Online on www.sportdata.org / Kickboxing Events APP", the same "by selection" line and "Remove online time table on www.sportdata.org". The local install asks "Do you really want to upload the time table to be available and visible for public on www.sportdata.org?" before the timetable upload. The knowledge base says to press yes, and that a pop up confirms the upload. Not clicked on the local test.

On SET 12.2.0 build 3 (local test, 6 Oct 2026) the three lines were only hovered, never clicked. "Upload timetable to SET Online on www.sportdata.org / Kickboxing Events APP" has the tooltip "Upload timetable to SET Online on www.sportdata.org".

![SET DTM - Dynamic Time Management, Upload timetable, tooltip](img/upload-online/09-timetable-upload-hover.png)

The by selection line reads "Upload timetable to SET Online on www.sportdata.org by selection / Kickboxing Ev" (cut off on screen). No tooltip showed for it in the test.

![SET DTM - Dynamic Time Management, Upload timetable by selection](img/upload-online/10-timetable-by-selection-hover.png)

"Remove online time table on www.sportdata.org" has the same text as its tooltip.

![SET DTM - Dynamic Time Management, Remove online time table, tooltip](img/upload-online/11-timetable-remove-hover.png)

## Check the event page

From the knowledge base: On the event page on sportdata.org, click the "Results" button to see the official results. Click "Draws" and then a category to see the uploaded draws. The "Timetable" section shows the uploaded timetable. It shows the individual matches only if the timetable was built from the match caller. If it was built only from categories and pools, the individual matches do not show.

Public sportdata.org page, 6 Oct 2026: after an upload, check on the public event page that the results and the timetable appear. No login is needed. The 7. Berner Cup 2026 event page is https://www.sportdata.org/kickboxing/set-online/veranstaltung_info_main.php?vernr=2871. Its tabs are INFORMATION, DOWNLOADS, CATEGORIES, ENTRIES, WAITING LIST, RESULTS and MEDAL STATISTIC. Above the tabs is a row of icon buttons, among them TIMETABLE.

### Results

Click the RESULTS tab.

![Event page, RESULTS tab](img/upload-online/14a-event-page-results-tab.png)

The results open on a new page (popup_main.php?popup_action=results&vernr=2871) headed RESULTS, with the line "7. Berner Cup 2026 - Results". Choose the category under SELECT A CATEGORY.

![Results, SELECT A CATEGORY](img/upload-online/14b-results-category-picker.png)

Below it, the table shows the category with RANK, NAME, CLUB and COUNTRY for each athlete.

![Results table for one category](img/upload-online/14c-results-table.png)

### Timetable and matchups

Click the TIMETABLE button. Its tooltip is "Timetable".

![Event page, TIMETABLE button](img/upload-online/15a-event-page-timetable-button.png)

The timetable opens at https://www.sportdata.org/setglinc/dtm/dtm_timetable.php?eventid=2871&system=kickboxing. It is headed "Event Schedule", with the event name, the day and one column per ring, Ring 1 to Ring 5.

![Event Schedule, Ring 1 to Ring 5](img/upload-online/15b-timetable-event-schedule.png)

Each block shows the category, the number of entries and the times. Some blocks show single matches, with the two athletes and "vs" between them.

![Timetable blocks with matchups](img/upload-online/15c-timetable-matchups.png)

The public event page has no separate Draws tab or DRAWS button. The matchups show in the Timetable. To check the uploaded draws, open the Timetable.

## Knowledge base steps

From the knowledge base article, lightly edited:

1. Go to Panels.
2. Click on SET Online.
3. Go to the drop down menu SET DTM - Dynamic Time Management. You can upload the entire timetable or by selection as well as remove the current timetable from online. Tip: Double click the top of the window where it first says SET Online Test / Test Events App to fully expand the window so you can see more.
4. Press yes to confirm that you want to publish and allow the public to see the timetable.
5. A pop up will confirm that the upload was successfully processed. If unsuccessful, check the internet connection.
6. In the draw, draw record, point table drop down list select either all draws or by selection.
7. Once completed, a confirmation pop up will appear.
8. To publish results go to the results drop down and select upload results.
9. Select the "Attention!" option for any necessary alerts.
10. Within the menu of the event page, find and click on the TIMETABLE section.
11. Click on the DRAWS button, then on the desired category.
12. On the event page, click on the results button.

On SET 12.2.0 build 3 the results line uploads at once, without a confirm step (Lucas).

On SET 12.2.0 build 3 (local test, 6 Oct 2026) the panel title reads "SET Online Kickboxing / Kickboxing Events APP", not "SET Online Test / Test Events App". The SET DTM - Dynamic Time Management lines for step 3 are shown under Timetable above.

Public sportdata.org page, 6 Oct 2026: for steps 10 to 12, TIMETABLE is an icon button above the tabs, there is no DRAWS button, and the results are under the RESULTS tab. See "Check the event page" above.
