# Architecture overview

## Desktop

Python application hosts the local UI and API. HTML/CSS/JavaScript provide the branded front end. Windows and macOS share the same app concept and most of the source structure.

## Android Pocket V2

Java Android activity loads the app's mobile UI assets in a WebView; the app has local offline note/photo storage and a paired, LAN-only communication path to the desktop API.

## Sync boundaries

**Validated on user devices:** Windows → Android idea+planner; Android → Windows basic idea.

**Implemented prototype but not verified end-to-end on user devices:** Windows ↔ macOS desktop sync via Google Drive folder.

**Not implemented:** Direct background Android ↔ Google Drive sync; a central always-on backend; fully automatic multi-device merge across all types of data.

Syncing local SQLite database files directly across devices can cause corruption and is not the proposed method. Keep separate local databases and exchange explicit changes/exports with a backup and conflict policy.
