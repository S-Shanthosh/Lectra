Import via Power Query — Data → Get Data → From File → From Text/CSV → select your Athena CSV
Click "Transform Data" (not Load) in the preview dialog
Change referenceno column type to Text — click the 123 icon on that column header → select Text → Replace current
Close & Load
Convert Table to Range — click inside the green/white table → Table Design tab (far right of ribbon) → Convert to Range → Yes
Format painter, choose any white column and fill all the columns except cdate, timestamp
Now format painter for  cdate, timestamp
select full excel cells, click on no table
Now excel is ready for scripting
