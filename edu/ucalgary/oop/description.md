How to check your work:
If your code is implemented correctly, the provided main will execute all of the demonstration tasks.

initializeConnection method must create a connection to the database, may not take in any arguments or return any values
        Must throw an SQLException if connection cannot be made
Use selectAllNames method to return a list of competitiors and a list of teachers (two separate calls)
         Must take in a String for the table name and return a String (mark deducted if incorrect)
         -1 if the content of the competitors list is incorrect
         -1 if the content of the teachers list is incorrect
Insert the given new competitor into the database
         Six arguments that match the competitor table, no return value (mark deducted if incorrect)
         Check to make sure the database has been updated with a new competitor
Insertion of the second given new competitor should fail and throw an IllegalArgumentException because the new student's teacher is not already registered in the database
        Check to make sure the competitor was not added
Insertion of the third given new competitor should fail and throw an IllegalArgumentException because the new student is outside of the valid age range
        Check to make sure the competitor was not added
Delete the specified competitor from the database
        Must take in the competitor's id as a String, no return value (mark deducted if incorrect)
        Check to make sure the competitor was deleted
Answer the following question in your demonstration:
        What data conflicts might arise when we try to delete an existing teacher?
Must show where all Statement, ResultSet, and Connection objects are closed. This may be in the close method or elsewhere in the code.


Tips:
Remember that each time you execute the given .sql file, the database will be reset. 
You should reset the database before each test run of your code.
You will cannot drop the database if you are using it - you will need to switch to using another database.

If you are having problems importing the SQL file, try removing the top lines which create the database, then running it after the database creation (from the tables).
