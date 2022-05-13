# Release Notes

## HCL Connections Desktop Plug-ins for Microsoft Windows

**Version 22.03.3081 (March, 2022) update**

- Resolved customer reported problems and bug fixes
    - Unable to upgrade to Windows Connections Desktop Plugin 22.03.3060 on non-English language systems.
    - Improved error messaging when Windows IP stack reports server unavailable error.
    - Windows 11 local draft popup notification has truncated text
    - Preferences panel shows save error after visiting but not changing server preferences for server with OAuth authentication
    - Crash when publishing local draft in community folder
    - Crash in trace utility when trying to save very large trace files
- Prompt to lock when opening files and prompt to unlock when publishing local changes. Behavior can be controlled by preference or administrator policy. Note: this does not apply to sync files.
- Initial sync performance improvements when processing thousands of files

## HCL Connections for Mac

**Version 22.03 (released March, 2022) update**

- Fixes an issue where unavailable actions may appear in the context menu shown when multi-selecting a mix of folders and files in the sync folder.
- Adds like, pin and follow actions for files and folders
    - Beta, English only - to use, click ‘Enable beta features’ in preferences
- Adds clickable link in properties panel to open log file location in Finder
- Initial sync performance improvements when processing thousands of files
- Customer reported problems and bug fixes:
    - Improve error message when failing to retrieve file properties
    - Make version text selectable and copyable in About box
    - Intermittent crash in authentication code

## HCL Connections Plug-ins for HCL Notes

**Apr 1, 2021**

- The Connections Notes Plugin now supports connecting to a Connections Multi-tenant server configurations.
    - To connect to a multi-tenant server, enter the server URL, select Advanced and choose OAUTH as the authentication type. After closing the preferences panel, you will be prompted to authenticate with a popup browser window.
    - Support for Connections v7
- Customer reported problems and bug fixes:
    - Fixed issue with closing Notes tabs when working with Activities
    - Some complex status updates can prevent status updates feed from loading
    - In status updates, thumbnails fail to load for unfurled URLs with long thumbnail URL length
    - Fix scenario in activities where Add Comment button on activity entry fails
    - Activity entry slide out panel Add Response button does not work
    - Status updates People search only worked for email addresses, not user names
