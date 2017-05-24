# SPanalytics
## Description
This script allows you to keep track of page hits on a specific SharePoint page. Every time a user loads the page, the script logs a 'hit' to a List on the same site.  
To keep the list from getting too big, the script creates a new record for each unique user and then counts the number of subsequent 'hits' over time. This is a great solution if you want to gauge the level of adoption of new solutions or to see if a page is ready to be retired due to inactivity.

## Instructions
1. Place analytics.txt in your site's 'Site Assets' folder
2. Create a new Custom List on your site. Give it a name that relates to the page you're wanting to track.
3. Make the following edits to the List:
  * Rename 'Title' to 'name'
  * Create a new (Single line of text) Column and name it 'email'
  * Create a new (Number) Column and name it 'visits
4. Open the new txt file and locate the line that reads as follows:  
  `<div id="analytics" value="CUSTOMLISTNAME"></div>`  
   _HINT: It's on Line 4_  
5. Change 'CUSTOMLISTNAME' to the exact name of the List you created in Step 2.
6. Save the file and Close it.
7. Add the txt file in a Content Editor WebPart on the page you want to track.
8. Watch the hits roll in!

**NOTE: This has only been tested in SharePoint 2010, so use with caution on any later versions (2013, 2016, etc...)**
