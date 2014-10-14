The project layout contains:

	1. Login page
	2. Availability Status
	3. Add Contact Details

The database currently being used is mysql. There are 2 tables with the following schemas:

	1. single_bed

| Field      | Type        | Null | Key | Default | Extra          |
|------------|-------------|------|-----|---------|----------------|
| id         | int(11)     | NO   | PRI | NULL    | auto_increment |
| name       | varchar(25) | NO   |     | NULL    |                |
| contact    | varchar(10) | NO   |     | NULL    |                |
| address    | varchar(30) | NO   |     | NULL    |                |
| start_date | date        | YES  |     | NULL    |                |
| end_date   | date        | YES  |     | NULL    |                |

	2. double_bed

| Field      | Type        | Null | Key | Default | Extra          |
|------------|-------------|------|-----|---------|----------------|
| id         | int(11)     | NO   | PRI | NULL    | auto_increment |
| name       | varchar(25) | NO   |     | NULL    |                |
| contact    | varchar(10) | NO   |     | NULL    |                |
| address    | varchar(30) | NO   |     | NULL    |                |
| start_date | date        | YES  |     | NULL    |                |
| end_date   | date        | YES  |     | NULL    |                |

The username and password for the sql server needs to be provided in the customer and home files. MySQL is being run on port 3307 (default port). While the login page as for now does a simple string comparison check directly in the code, all other operations are in sync with the sql server.

