# Go offline

Checked on SET OVR 12.2.0 build 3, 3 Oct 2026. The Settings window parts were checked again on 6 Oct 2026 on a local copy.

There is no Go offline command in File, Settings, or Tools.

![File menu, no Go offline](img/go-offline/02a-file-menu.png)

![Settings menu: Settings (Ctrl+P), Email Smtp, Language](img/go-offline/02b-settings-menu.png)

![Tools menu, no Go offline](img/go-offline/02c-tools-menu.png)

The Settings menu has three items: Settings (Ctrl+P), Email Smtp, and Language.

The local server is the connection window that opens when SET starts. Red boxes mark the control.

## Connect to the local database

Start SET. On 6 Oct 2026 (build 3, local test) two windows came before the connection window:

- Select network interface, with a network dropdown, Do not ask again, and OK. Click OK.

  ![Select network interface, OK](img/go-offline/01a-select-network-interface.png)

  The dropdown lists the network interfaces of the PC with their addresses. On SET 12.2.0 build 3 (local test, 6 Oct 2026) it listed tailscale0, docker0 and enp0s4. The addresses are blurred in the screenshot.

  ![Network interface list, addresses blurred](img/go-offline/01a2-network-interface-list.png)

- SET OVR License Grant and Restriction. Click OK.

  ![SET OVR License Grant and Restriction, OK](img/go-offline/01b-license.png)

The connection window is titled with the SET version, for example SET v 12.2.0 build 3 (2026-08-17 22:26 CET). The group inside it is labelled Connection Settings.

Choose **Use local / network database**.

![Use local / network database](img/go-offline/01c2-use-local-radio.png)

![Connection Settings, whole window](img/go-offline/01c-connection-settings.png)

The other choices on that window are Use integrated database, Use SET-Online database, and Import Database-Backup from SQL file.

With local / network selected, the form shows the fields below, from top to bottom. The close-ups are from SET 12.2.0 build 3 (local test, 6 Oct 2026). The fields were hovered, not changed, except Database Type in the test on [Local server without MariaDB](local-server.md).

ONLINE System / TYPE shows Kickboxing [www.sportdata.org/kickboxing]. Kickboxing is `www.sportdata.org/kickboxing`.

![ONLINE System / TYPE, Kickboxing](img/go-offline/01c3-online-system-type.png)

Database Type offers only two values: H2 - Integrated DB Server and MYSQL - External DB Server. At the Berner Cup the venue used MYSQL - External DB Server on port 27000. See [Local server without MariaDB](local-server.md). On SET 12.2.0 build 3 (local test, 6 Oct 2026): the restored local copy uses H2 - Integrated DB Server.

![Database Type values](img/go-offline/01d-database-type.png)

Database holds the database name. Next to it is the "Local H2 Databases..." dropdown. On the local copy the name was bernercup2026_b2.

![Database and Local H2 Databases...](img/go-offline/01c4-database-local-h2.png)

On SET 12.2.0 build 3 (local test, 6 Oct 2026): Server showed localhost and Port showed 3306, greyed out with H2. These are local defaults, not a correction of the venue port 27000.

![Server localhost, Port 3306 greyed out](img/go-offline/01c5-server-port.png)

DB-Username showed root, greyed out with H2. Next to it is DB-Password. Below them is "Remember password on next login", ticked on the local copy. The DB-Password field is blurred in the screenshot.

![DB-Username, DB-Password, Remember password on next login](img/go-offline/01c6-db-username-password.png)

Language showed english. Below it is the "License Manager" button.

![Language english, License Manager](img/go-offline/01c7-language-license.png)

Settings has three buttons: Export, Import and Remote Import. None of them was clicked in the test.

![Settings: Export, Import, Remote Import](img/go-offline/01c8-settings-export-import.png)

Create DB User for remote access stayed greyed out. It was greyed out again on 6 Oct 2026 with H2. With MYSQL - External DB Server it becomes active. Do not use the names already in the boxes. They are whatever this install last stored, not the event setup. Click Test connection before Connect.

![Test connection, Create DB User for remote access (greyed out), Connect](img/go-offline/01e-connection-buttons.png)

On SET 12.2.0 build 3 (local test, 6 Oct 2026): Test connection with H2 - Integrated DB Server and bernercup2026_b2 opened an "Attention!" box: "Connecting the database was successful". Click OK, then Connect.

![Attention!, Connecting the database was successful, OK](img/go-offline/01e2-test-connection-ok.png)

On SET 12.2.0 build 3 (local test, 6 Oct 2026): Connect with H2 - Integrated DB Server opened the SET Login window. The full local login is below.

**Warning: do not pick Use integrated database to reopen a restored copy.** On SET 12.2.0 build 3 (local test, 6 Oct 2026): picking Use integrated database greys out the database fields. Connect then opens SET's default integrated database, not the restored event. Logging in with the event's user then fails with Wrong SET-Username or SET-Password!. To reopen a restored local copy, keep Use local / network database with H2 - Integrated DB Server and the copy's database name.

![Use integrated database greys out the database fields](img/go-offline/01f-integrated-greyed.png)

The SET Login window has SET-Username, SET-Password, Remember password on next login, and the modes Registration Mode, RING Mode, Administration Mode, Referee Mode, and Terminal Mode, with Log in and Cancel. Choose Administration Mode for the checks below, then click Log in. On SET 12.2.0 build 3 (local test, 6 Oct 2026): the username and password were already filled in because "Remember password on next login" was ticked at the last login. The login fields are blurred in the screenshot.

![SET Login, Administration Mode, Log in](img/go-offline/01g2-set-login-admin.png)

The "Event data" window opens. Click the event row, here 7. Berner Cup 2026 (2026.10.04, SWITZERLAND, Id 2871), then click Next. The main window opens with Administration Mode at the start of the title bar. The Main Tree Menu shows 7. Berner Cup 2026 (local).

![Event data, 7. Berner Cup 2026, Next](img/go-offline/01h-event-data.png)

## Checks from the process document

Open Settings, then Settings (Ctrl+P). You need to be in Administration Mode.

Administration Mode shows at the start of the title bar and on the Welcome panel.

![Administration Mode in the title bar](img/go-offline/02d-administration-mode-title.png)

![Administration Mode on the Welcome panel](img/go-offline/02e-administration-mode-welcome.png)

### User

Open the User tab.

![User tab in the Settings tab bar](img/go-offline/03-user-tab.png)

In the User section, click User / Password.

![User / Password in the User section](img/go-offline/03b-user-password.png)

A dialog titled User-Management opens. Its heading is Add new user/Change password. It has two checkboxes, Change password and Add new user, and the buttons OK and Close.

Tick Add new user. The login is the one from the backup.

![User-Management, Add new user](img/go-offline/04-user-management.png)

On SET 12.2.0 build 3 (local test, 6 Oct 2026): ticking Add new user only ticked the checkbox. No form fields appeared. Unticking it closed the dialog. OK was not clicked and no user was created.

![Add new user ticked, no form fields](img/go-offline/04b-add-new-user-ticked.png)

### Seeding

Open the Seeding tab.

![Seeding tab](img/go-offline/05-seeding-tab.png)

The Seed Mode section lists Mode 1 to Mode 7. The process document says Mode 3. That row is `Mode 3:[1,8,5,4:3,6,7,2]`. Mode 2 was already selected on this screen. It was not changed. On 6 Oct 2026, Mode 2:[8,4,6,2:7,3,5,1] was still the selected one.

![Mode 3](img/go-offline/06-mode3.png)

### Draw record

Open the Draw / Draw record tab.

![Draw / Draw record tab](img/go-offline/07-draw-tab.png)

The block is Club / Nation display options. The process document says Club/Nat. The matching label on this screen is `(Club,Nat)`. `(Club,Nation)` is the similar one beside it. The selected radio was left as it was. The full list is (Cl), (Club), (Club,Nation), (Club,Nat), (Cl,Nat), none, (Club,FA), (Cl,FA), (FA), (Federal Association), (Nat), and (Nation). On the local copy, (Cl) was selected.

![(Club,Nat)](img/go-offline/08-club-nat.png)

### Area names

Open the Monitor / DTM Area Name Replace tab.

![Monitor / DTM Area Name Replace tab](img/go-offline/09-area-tab.png)

Fill Name Original and Name New, then Add. The process document example is Ring 1 replaced with Tatami 1. The fields are Name Original: and Name New: along the bottom, with Add at the bottom right and Remove at the bottom left. The venue list at the Berner Cup was not empty. See [Wrong name monitor (workaround)](wrong-name-monitor.md).

![Name Original, Name New, and Add](img/go-offline/10-area-fields.png)

On SET 12.2.0 build 3 (local test, 6 Oct 2026): the list was empty on the local copy. Ring 1 went into Name Original and Tatami 1 into Name New. Then Add.

![Name Original Ring 1, Name New Tatami 1, Add](img/go-offline/10a-area-fields-filled.png)

After Add the list showed one row, Ring 1:Tatami 1.

![The new row Ring 1:Tatami 1](img/go-offline/10b-area-row-added.png)

To take a row off, select it and click Remove. The test row was removed this way.

![Row selected, Remove](img/go-offline/10c-area-row-remove.png)

After Remove the list was empty again and Remove was greyed out.

![Empty list, Remove greyed out](img/go-offline/10d-area-list-empty-again.png)

### Close Settings

The Settings window has no Cancel or Close button. Close it with the X in its title bar.

![X in the Settings title bar](img/go-offline/11-settings-close-x.png)

On SET 12.2.0 build 3 (local test, 6 Oct 2026): closing with the X gave no save prompt.

Wrong name: monitor on the display is a separate workaround: [Wrong name monitor (workaround)](wrong-name-monitor.md).
