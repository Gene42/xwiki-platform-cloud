Introduction
============

This module builds a WAR that can be deployed on Amazon Beanstalk. It uses the MySQL driver for storing data in the database.

When starting the Beanstalk environment you need to allocate an `xwiki` database on Amazon RDS and define the following properties in the Beanstalk panel:

* `JDBC_CONNECTION_STRING` need to be something like `jdbc:mysql://AMAZON_RDS_HOST/xwiki?useServerPrepStmts=false&amp;useUnicode=true&amp;characterEncoding=UTF-8` where `AMAZON_RDS_HOST` is the host name of a previously allocated database on Amazon RDS
* `PARAM1` is the user name for accessing the database on Amazon RDS
* `PARAM2` is the user password for accessing the database on Amazon RDS
