# Local server without MariaDB

Confirmed on the Berner Cup PCs on 3 Oct 2026. SET was v12.2.0 build 2.

## Database mode

The working database was not MariaDB. SET was set to Use local / network database, Kickboxing, MYSQL - External DB Server.

The port was 27000.

The database name that opened 7. Berner Cup 2026 was 2026bernercup. A database field of mydb opened 1. Alpen Open 2026 instead. Confirm the event list says 7. Berner Cup 2026 before continuing.

On SET 12.2.0 build 3 (local test, 6 Oct 2026): the window title does not show the event name. Check the top node of Panels, then Main Tree Menu. On the local copy it read 7. Berner Cup 2026 (local). The EVENT column of the Events panel shows the same name, cut off as 7. Berner C...

![Main Tree Menu top node with the event name](img/local-server/01-main-tree-root.png)

![Events panel, EVENT column](img/local-server/02-events-panel.png)

## Server PC

On the server PC (Haupttisch), Server was localhost. The DB user was root. The SET login that worked on the scale PC was the username from the database backup. That login was not the Windows user and was not the admin login.

ipconfig on the Haupttisch showed IPv4 192.168.x.125, mask 255.255.255.0, and Wi-Fi disconnected. That address was then changed to 192.168.x.10 so the scale PC could reach it.

The scale PC address seen earlier was 192.168.x.227. The router was 192.168.x.254.

## Scale PC test

The Test connection that succeeded used Server 192.168.x.10, port 27000, database 2026bernercup, and user root. Do not click Connect until Test connection succeeds.

## Address already in use

An earlier PC was already at 192.168.x.10. That PC did not work. Private and Public firewalls were enabled, and nothing was listening on port 27000. Do not use that PC as the setup. The working server was the Haupttisch after its address was set to 192.168.x.10.

## SQL import

The SQL file used was 2026bernercup.sql. It was imported with Import Database-Backup from SQL file. A finished import log said Server localhost, Port 27000, DB-Username root, and created database 2026bernercup.
