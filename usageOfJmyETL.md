# Introduction #

Here is the main usage of jmyetl-1.0.2.  It mainly focus on the data import/export from one DBMS to other DBMS. Such as FrontDB/PostgreSQL, CUBRID, Sybase ASE/ASA, Oracle, MySQL, DB2, SQLServer, Access and even SQLite.

It's very useful for the multiple datasource support sometimes.

# Details #
  1. From the download location, decompress the zip file of jmyetl-1.0.2.
  1. **Edit the ini file:  jmyetl.ini,  adjust the value of vm.location to your {JAVA\_HOME}\jre\bin\server\jvm.dll**.   [note:](please.md) for now, it only supports 32-bit jdk. Even you are in 64-bit OS, please also use 32-bit jdk1.6 and above. We recommend use jdk1.6. The jdk can be any unzipped version. Because I implement it and test it in jdk1.6 by default.

  1. **For the jmyetl.ini, you can also add the following value in new lines**.
    * vmarg.1=-Xms64M
    * vmarg.2=-Xmx512M
  1. Open JmyETL.exe, fill in the {host}, {database}, {port} information for the
> > source db and target db. Click the test connect to ensure they are both connected.
  1. click start import.
  1. For Access Database, you need not create the mdb file in advance. If it doesn't exist, the tool will create it for you. 如果Access数据库文件不存在，工具会为你自动创建一个mdb数据库文件。

See the sample picture:

![http://hisql.googlecode.com/files/pic0.jpg](http://hisql.googlecode.com/files/pic0.jpg)