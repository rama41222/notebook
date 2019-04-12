#### VARCHAR VS NVARCHAR

* Nvarchar stores UNICODE data.
* If you have requirements to store UNICODE or multilingual data, nvarchar is the choice
* Varchar stores ASCII data and should be your data type of choice for normal use.

##### Regarding memory usage, 
* nvarchar uses 2 bytes per character
* varchar uses 1.

##### Joining 
* JOINing a VARCHAR to NVARCHAR has a considerable performance hit.

*Using nvarchar over vachar will stop unicode conversions.*
