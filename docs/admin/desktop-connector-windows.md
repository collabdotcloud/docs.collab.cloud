**Removing the Old configuration**

There are some known issues removing the old Connections Cloud configuration from the desktop connector. The standard process is the following.

Go to Windows Explorer, find the Connector and connected sites in the left navigation pane ( mostly at the bottom), right click on the site you want to remove and click "Disconnect form Site"

**Files are in use error**

This works in most cases, but you can get a warning that it can't be removed because files are in use. The most successful solution we have found so far is to open taks manager, restart the Windows Explorer task, and immediately remove as described above, there should be no error
Same would happen if you would try this immediately after booting the pc

**Pinned Folders in Windows Explorer**

Please make sure you remove all pinned folders pointing to IBM Smartcloud before you removed the Smartcloud configuration from the Desktop connector, it is very hard to remove them afterwards
