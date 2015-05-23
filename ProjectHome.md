## JMyETL 1.0.8 ##
Fix the issue of :
  1. Update the Readme.
  1. Fix the bug of mysql column type : TINYINT. When the source table from mysql includes TINYINT column type, the target database PG will have issue. Fix it here.

## JMyETL 1.0.6 ##
Fix the issue of :
  1. "Test Connect" doesn't sound right. It's better to translate it as "Test Connection". This is what other DB applications use.
  1. When the JMyETL is running under jdk1.7, there will be a UI deadlock. It only happens under jdk1.7.  Fix it here.
  1. Patch steps:
> > Just download the jmyetl.jar from jmyetl-1.0.6.zip and overwrite this file on the decompressed jmyetl-1.0.5.zip.

## JMyETL 1.0.5 ##
  1. Update the README of JMyETL for jdk version(32bit, 1.6 above)
  1. Cancel the license restriction for the JMyETL on all the DBMS. The target DBMS can be all the DBMS types.
  1. Fix some internal issues about import/export.

There is a known issue here to be fixed by JMyETL side or on CUBRID side.
When the source DBMS is cubrid and the target DBMS is other kinds of DBMS,  if the target db failes to connect, it will throw CUBRID driver/connection exception. Please ignore it. Please ensure the target DBMS connect successfully in advance.

## JMyETL 1.0.4 ##

> 开始支持中文界面，支持第三方开源数据库CUBRID，并提供对SQLServer和DB2的支持。
> The latest version is 1.0.4.  Add new support for CUBRID (another opensource DBMS from Korea). Add support for SQLServer, DB2.
> The detail usage, please refer to: http://code.google.com/p/hisql/wiki/usageOfJmyETL
> For CUBRID, you can access it via: http://www.cubrid.org

## JMyETL 1.0.3 ##
> The latest version is 1.0.3.  Support Sybase ASE/ASA, MySQL, Oracle, Access, PostgreSQL(FrontDB) export and import to each other.
> The detail usage, please refer to: http://code.google.com/p/hisql/wiki/usageOfJmyETL

### Design Goal: ###
> The table export and import between the following DBMS
  * MySQL --> Sybase ASE/ASA, Oracle, Access, PostgreSQL, SQL Server, DB2, SQLite, CUBRID
  * Sybase ASE --> Sybase ASA, MySQL, Oracle, Access, PostgreSQL, SQL Server, DB2, SQLite, CUBRID
  * Sybase ASA --> Sybase ASE, MySQL, Oracle, Access, PostgreSQL, SQL Server, DB2, SQLite, CUBRID
  * Oracle --> Sybase ASA, Sybase ASE, MySQL, Access, PostgreSQL, SQL Server, DB2, SQLite, CUBRID
  * Access --> Sybase ASE, Sybase ASA, MySQL, Oracle, PostgreSQL, SQL Server, DB2, SQLite, CUBRID
  * PostgreSQL --> Sybase ASE, Sybase ASA, MySQL, Oracle, Access, SQL Server, DB2, SQLite, CUBRID
  * SQL Server --> Sybase ASE, Sybase ASA, MySQL, Oracle, PostgreSQL, Access, DB2, SQLite, CUBRID
  * DB2 --> Sybase ASE, Sybase ASA, MySQL, Oracle, PostgreSQL, SQL Server, Access, SQLite, CUBRID
  * SQLite --> Sybase ASE, Sybase ASA, MySQL, Oracle, PostgreSQL, SQL Server, DB2, Access, CUBRID
  * CUBRID --> Sybase ASE, Sybase ASA, MySQL, Oracle, PostgreSQL, SQL Server, DB2, Access, SQLite
> When the target DBMS is PostgreSQL(hisql), CUBRID or Access, it's totally free to use. The source DBMS can be any kind of DBMS in the above list.
### Download: ###
  * http://code.google.com/p/hisql/downloads/list (for now)

### Update History: ###
  * 2012.8.5, submit the updated version: 1.0.5 of jmyetl.
  * 2012.6.19, submit the updated version: 1.0.4 of jmyetl, fix some bugs. Add Chinese language support. Add CUBRID as source db and target db. Add DB2 as source db and conditional target db(need license). It's totally free when the target DBMS is PostgreSQL(Dataware), CUBRID or Access.
  * 2012.6.10, submit the updated 1.0.3 of jmyetl. Adding the support of SQLServer and SQLite database.
  * 2012.6.9, submit the initial alpha version: 1.0.2 of jmyetl.  Support PostgreSQL, Sybase ASA/ASE, MySQL, Access, Oracle import and export.

## Our Contact info: ##
  * hexiong AT gmail.com
  * Or you can find me on http://blog.csdn.net/iihero and http://www.sql9.com
  * To keep the next developement of hisql related projects, any donation is appreciated: Donation: http://www138.com/donation.htm