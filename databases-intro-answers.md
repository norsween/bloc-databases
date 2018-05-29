Exercises:

1)What data types do each of these values represent?

"A Clockwork Orange"     	(STRING)
42  				(INTEGER)
09/02/1945  			(DATE)
98.7  				(FLOAT)
$15.99				(CURRENCY)

2) Explain when a database would be used. Explain when a text file would be used.

	A: Databases would be used when applications can create and store data on the user’s behalf.  A text file would be used when the information contained therein don’t need to be searched nor is there an application interfacing with it.

3) Describe one difference between SQL and other programming languages.

	A: SQL is a declarative rather than a procedural language. It is used to write what we want to find without telling the system on how to find it.  It’s also used to access a database. Other programming languages are procedural languages, i.e., these instruct the operating system or the application about the actual steps to take to perform a function.  

4) In your own words, explain how the pieces of a database system fit together at a high level.

	A: At a high level, a database is a collection of rows and columns of data, i.e. data represented in tabular form. The column names are used to label each row of data. 

5) Explain the meaning of table, row, column, and value.

	A: A table is a conceptual structure of how data is represented in terms of columns and rows. Rows make up a complete conceptual unit. Columns define what the data represent. A particular value denote some piece of information that the column name describes.

6) List three data types that can be used in a table.

	A: string, integer, date

7) Given this payments table, provide an English description of the following queries and include their results:

     SELECT date, amount
     FROM payments;

	A: Get and display the date and amounts of all rows from the payments table.

		date			amount
		2016-05-01		1500
		2016-05-10		  37
		2016-05-15		 124.93
		2016-05-23		  54.72


     SELECT amount
     FROM payments
     WHERE amount > 500;

	A: Get and display the amount only of all payments where amount > 500.

		amount
		1500


     SELECT *
     FROM payments
     WHERE payee = 'Mega Foods';

	A: Get and display all the column values of payments where payee is ‘Mega Foods’

		date		payee		amount		memo
		2016-05-15	Mega Foods	124.93		Groceries


8) Given this users table, write SQL queries using the following criteria and include the output:

	The email and sign-up date for the user named DeAndre Data.

		A: select email, signup from users where name='DeAndre Data';

				email			signup
			datad@comcast.net		2008-01-20


	The user ID for the user with email 'aleesia.algorithm@uw.edu'.

		A:  select userid from users where email = 'aleesia.algorithm@uw.edu';

				userid
				  1


	All the columns for the user ID equal to 4.

		A: select * from users where userid = 4;

		userid		name		email			signup
			
		4		Brandy Boolean	bboolean@nasa.gov	1999-10-15
