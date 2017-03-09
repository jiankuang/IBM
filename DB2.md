# DB2 System, Instance & Database
* DB2 Database is where you store and retrieve data
* DB2 instance is a run time entity comprising multiple database and their configuration
* DB2 instance is also referred as database manager (DBM)
* DB2 System is a complete DB2 environment comprising multiple DB2 instances and databases
* 2 Configuration files
  - DB CFG for Database
  - DBM CFG for Instance
  
## Instance Creation on Windows
* `db2icrt MYINST -p C:\Users\jian\IBM\MYINST`
* Instance created under folder `C:\Users\jian\IBM\MYINST`

# CLI Commands
* Windows -> Run -> `DB2CMD` is the CLI we need to work on
* `BD2ILIST` list all the DB2 instances on this machine
* `DB2 GET INSTANCE` get the current DB2 instance
* `GET DBM CFG` get configuration file
* `SET DB2INSTANCE=name_of_instance` set the current DB2 instance
* `DB2 LIST DB DIRECTORY` list all the databases in the current instance
* `DB2SET -ALL` get the setting info of the current instance
