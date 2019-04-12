### Boolean Datatype in mssql

Bit can take a value of `1, 0, or NULL.`

* The SQL Server Database Engine optimizes storage of bit columns. 
* If there are 8 or less bit columns in a table, the columns are stored as 1 byte.
* If there are from 9 up to 16 bit columns, the columns are stored as 2 bytes, and so on.
* TRUE is converted to 1 and FALSE is converted to 0.
* Converting to bit promotes any nonzero value to 1.

