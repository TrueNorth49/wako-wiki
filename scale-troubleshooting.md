# Scale and scanner troubleshooting

Confirmed on the Berner Cup PCs on 3 Oct 2026. SET was v12.2.0 build 2.

## Serial devices

The scanner and the scale are separate USB serial devices (FTDI). In Device Manager the working serial settings were 9600, 8 data bits, parity none, 1 stop bit, and flow none.

SET has two sections: Serial interface (Barcode Scanner only) and Serial interface (TV, Scale, OVR, Horn). Both used 9600, 8, 1, None.

Both sections are in Panels, then Data services. Expand each section by its title.

![Panels, Data services](img/scale-troubleshooting/01-panels-data-services.png)

![Serial interface (TV, Scale, OVR, Horn)](img/scale-troubleshooting/02-serial-scale.png)

![Serial interface (Barcode Scanner only)](img/scale-troubleshooting/03-serial-barcode.png)

On SET 12.2.0 build 3 (local test, 6 Oct 2026): both sections showed 19200, 8, 1, None. That is the local copy's default. It does not change the venue value of 9600. The scale section has Open port, a COM dropdown, and the Scale: Ignore values below 1.0 kg checkbox. The barcode section has COM Port - Settings with Open port and a COM dropdown, Custom Command with Send Command, Enable Scanner beep on error, and a scanner dropdown set to Datalogic.

In the local test no serial device was connected and no port was open. The COM dropdowns were empty, and Open port, COM and the 19200 baud field were greyed out. The local copy cannot show the venue setting. At the venue, check both sections and set 9600 if they show anything else.

![Serial interface (TV, Scale, OVR, Horn), Open port, COM and 19200 greyed out](img/scale-troubleshooting/15-scale-port-greyed.png)

![Serial interface (Barcode Scanner only), Open port, COM and 19200 greyed out](img/scale-troubleshooting/16-barcode-port-greyed.png)

## Port assignment

The assignment that worked was scanner on COM5 and scale on COM6. The scale needed a power cycle after the port move. An earlier wrong assignment was scanner on COM3 and scale on COM5.

On SET 12.2.0 build 3 (local test, 6 Oct 2026) the COM dropdowns were empty, so COM5 and COM6 can only be checked at the venue.

The scale option Ignore values below 1.0 kg was checked. On screen it reads Scale: Ignore values below 1.0 kg. It sits under Serial interface (TV, Scale, OVR, Horn) in Data services.

## Weigh-in window

To open Weight / size control, open Panels, then Main Tree Menu. Right-click Individual / Team Entries and choose Weight / size control.

![Panels, Main Tree Menu](img/scale-troubleshooting/04-panels-main-tree-menu.png)

![Individual / Team Entries, Weight / size control](img/scale-troubleshooting/05-weight-size-control-menu.png)

The QR reader default action that matched the Sport Data page was Weight / size control connected with the scale. Keep that window open. A scan then opens the athlete. Access Control is the wrong window.

On SET 12.2.0 build 3 (local test, 6 Oct 2026): the menu is "QRCode Reader". It has "QRCode Reader from Barcode Scanner" and "QRCode Reader from Webcam". Choose "QRCode Reader from Barcode Scanner".

![QRCode Reader, QRCode Reader from Barcode Scanner](img/scale-troubleshooting/11-qrcode-reader-menu.png)

The window has one button per mode, for example "Access Control", "Entries", "Weight / size control" and "Weight / size control - Connected with Scale".

![Weight / size control - Connected with Scale button](img/scale-troubleshooting/12-barcode-scanner-modes.png)

At the bottom is "Default Action". Pick "Weight / size control - Connected with Scale", not "Access Control".

![Default Action, Weight / size control - Connected with Scale](img/scale-troubleshooting/13a-default-action-scale.png)

![Default Action, Access Control is the wrong choice](img/scale-troubleshooting/13b-default-action-access-control.png)

The field then reads "Weight / size control - Connected with Scale". "Exit Barcode Scanner Mode" is below it.

![Default Action set, Exit Barcode Scanner Mode](img/scale-troubleshooting/14-default-action-set.png)

The console showed NO EOT found while the scanner was on the wrong port. After the COM swap it showed BarCode Data Received and BarCode EOT found.

The Message Console is the panel under the Main Tree Menu. It is also an item in Panels. On SET 12.2.0 build 3 (local test, 6 Oct 2026) no scanner was connected, so these lines did not show. The status line at the bottom of the window read "[INFO] Messages found 0". The console text is blurred in the screenshot.

![Message Console panel and status line Messages found 0](img/scale-troubleshooting/17-message-console.png)

## Weights that do not stay saved

If a weight shows on screen and the Weighed status does not stay saved, check the category limits. On the Weight / size control list, Min. Wei. and Max. Wei. were 0.0 on every visible row, and the status stayed Pending. The Sport Data automatic weigh-in page says the status changes to Weighted only when the stable weight is inside the category range, and Min. Weight must not be zero.

![Min. Wei. and Max. Wei. were 0.0 and status stayed Pending.](img/weight-list-min-max-zero.jpg)

On SET 12.2.0 build 3 (local test, 6 Oct 2026): the column titles are cut off. Mi... has the tooltip Min. Weight. M... has the tooltip Max. Weight. En... has the tooltip Entries Status. Most rows show a minimum of 1.0 and a maximum such as 63.0, 69.0 or 74.0. Two rows show 0.0 and 0.0 with a yellow status. The footer counts the statuses, for example P: 11 (4%) and W: 223 (95%). A row with 0.0 and 0.0 means the category limits are not set.

![Min. Weight column and 0.0 rows](img/scale-troubleshooting/06-min-weight.png)

![Max. Weight column and 0.0 rows](img/scale-troubleshooting/07-max-weight.png)

![Entries Status column, yellow rows](img/scale-troubleshooting/08-entries-status.png)

![Status counts P and W](img/scale-troubleshooting/09-status-footer.png)

At the venue on v12.2.0 build 2, Panels did not list Competitor Categories.

![Panels on v12.2 did not list Competitor Categories.](img/panels-no-competitor-categories.jpg)

On SET 12.2.0 build 3 (local test, 6 Oct 2026): Panels does list Competitor Categories, second from the top.

![Panels, Competitor Categories on build 3](img/scale-troubleshooting/10-panels-competitor-categories.png)

The Sport Data page says that panel is under Panels after an administration-mode login, or it is already open. The click that fills the zero limits on this build is not confirmed yet.

If weights are not saving, look at Min. Wei. and Max. Wei. If they are 0.0, the category limits are not set.
