# zotero-word-for-wine-linux-integration
Zetoro plugin for Word on Wine under Linux. Currently I have only made the plugin for standalone Zotero, following the instructions fdeboiss of Zotero Forum [1].

Please find the version of Zotero.dotm that corresponds to your Zotero's version, and copy it to .wine/drive_c/users/%user_name%/Application\ Data/Microsoft/Word/STARTUP/.

If you would like to create Zotero.dotm by yourself, following the following instruction from fdeboiss:

- backup somewhere the .wine/drive_c/users/%user_name%/Application\ Data/Microsoft/Word/STARTUP/Zotero.dotm (%user_name% is your user name)
- copy Zotero.dotm somewhere where you can edit it (e.g. in you home directory)
- open the copy from Word menu
- go to view --> macro --> view macros
- clic modify on any selected Zotero macro to edit
- remove at line 146 & " -ZoteroIntegrationDocument """ & name$ & """"
- replace at lines 162-165 Mozilla Firefox\firefox.exe by Zotero Standalone\zotero.exe
(For 5.x versions, replace Mozilla Firefox\firefox.exe by Zotero\zotero.exe).
- save the macro edition
- replace the old Zotero.dotm with the new in .wine/drive_c/users/%user_name%/Application\ Data/Microsoft/Word/STARTUP/

[1] https://forums.zotero.org/discussion/12426/word-intergration-with-wine/p3
