#### What it is
 - SuperSync is an <a href="http://home.opml.org/">OPML Editor</a> tool that runs on any computer that has access to your Dropbox folder. You can run it on your desktop computer (I do). It keeps folders in sync with locations on Amazon S3. You can have as many sharepoints as you want. You set it up by editing the config.root object database. It's how I keep the Fargo Docs site in sync with its location on S3. 

#### How to install
 - Choose Tool Catalog from the Misc menu in the OPML Editor. 

 - Click on the Install link next to SuperSync. Click on OK to all confirmation prompts.

#### How to set up
 - At this time you have to create new tables for sync points by hand in the object database.

 - Jump to <a href="http://static.scripting.com/larryKing/images/2013/12/06/configSuperSync.gif">config.superSync</a>, and create a new sub-table of the points table. Wait till the top of the minute, and a background script will initialize the table for you.

 - Open the table and open its prefs sub-table, and fill in the three parts <a href="http://static.scripting.com/larryKing/images/2013/12/06/prefsTable.gif">like this</a>.

 - When you're ready to start syncing change config.superSync.prefs.enabled to true. 

 - When syncing happens you should <a href="http://static.scripting.com/larryKing/images/2013/12/06/logOutline.gif">see an outline</a> window open showing you the files it's uploaded.

#### Maintenence
 - You should update the tool from time to time.

 - The log outlines are automatically cleared every night.
