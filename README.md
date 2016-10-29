# DBManager

This code stemed from the idea of how to manage SQL updates to an exsisting database. I aproached this by thinking about how a large scale project with users who don't know SQL would automatically make changes to the database. My solution was a system that uses patches to make sequential changes to the database that are automatically run and managed by an interface. 

## What it does
A folder with sql files is scanned and parsed and it is determined if there are any new files that have not been run against their database. DBManger creates it's own database for keeping a record of changes to the databases that it manages. When a new file is found that hasen't been run against it's database, DBManager can alert you. There is currently a method for adding a drop down header warning that should go on a site administration page. The software doesn't currently let you automatically apply all new patches. 
