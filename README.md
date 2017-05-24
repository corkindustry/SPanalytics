# SPanalytics
A script that tracks hits on a SharePoint page.

## Instructions

### CEWP Method
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
