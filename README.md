# BackupBaikal
BackupBaikal for Windows

## Purpose
Backups Contacts and Calendars from Baikal or Nextcloud to local ics and vcf files.
Multiple calendars and contacts can be backuped. Files are stored in the same folder.

## Installation
1. Create Folder
2. Copy .exe and .conf to a folder
3. Edit configuration file
4. Create scheduled task running the exe without arguments

## Configuration
```
{
 "calendars": [
  {"url":"https://dav.yourdomain.com/remote.php/dav/calendars/<youruser>/<yourcalendar>/?export",
   "user":"<username>",
   "pass":"<password>",
   "name":"<nameofcalendar>"},
   {"url":"https://dav.yourdomain.com/remote.php/dav/calendars/<youruser>/<yourcalendar>/?export",
   "user":"<username>",
   "pass":"<password>",
   "name":"<nameofcalendar>"}
 ],
 "contacts": [
 {"url":"https://dav.yourdomain.com/remote.php/dav/addressbooks/users/<youruser>/<yourcontacts>/?export",
   "user":"<username>",
   "pass":"<password>",
   "name":"<nameofcontacts>"},
   {"url":"https://dav.yourdomain.com/remote.php/dav/addressbooks/users/<youruser>/<yourcontacts>/?export",
   "user":"<username>",
   "pass":"<password>",
   "name":"<nameofcontacts>"}
 ]
}
```
### Nextcloud
Calendar: https://dav.yourdomain.com/remote.php/dav/calendars/<youruser>/<yourcalendar>/?export

Contacts: https://dav.yourdomain.com/remote.php/dav/addressbooks/users/<youruser>/<yourcontacts>/?export
