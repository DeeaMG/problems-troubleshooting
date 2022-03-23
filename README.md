# problems-troubleshooting

A little repository with small problems I encountered, and their solution.

 ***1. OneDrive Syncing Error***
> **Error 0x80071129: The tag present in the reparse point buffer is invalid.**
This error occurs when OneDrive fails to sync the files correctly, and you can't open/delete the folder/file

***Solution:***
 - Open **`cmd`** as Administrator.
 - Type **`chkdsk c: /r /f`**.
 - If **`chkdsk`** cannot lock the drive, a message appears that asks you if you want to check the drive the next time you restart the computer, type Y.
 - Restart your PC.
 - Now you can open/delete the files/folders.

	This command checks the file system and file system metadata of a volume for logical and physical errors.
**`/f`** - Fixes errors on the disk.
**`/r`** - Locates bad sectors and recovers readable information.
