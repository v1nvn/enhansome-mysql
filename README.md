# awesome-mysql

A curated list of awesome MySQL free and opensource software, libraries and resources. [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) ⭐ 438,154 | 🐛 70 | 📅 2026-01-28

This list accepts and encourages pull requests. See [CONTRIBUTING](https://github.com/shlomi-noach/awesome-mysql/blob/master/CONTRIBUTING.md) ⭐ 2,544 | 🐛 14 | 🌐 Python | 📅 2026-02-15

### Contents

* [Awesome MySQL](#awesome-mysql)
  * [Analysis](#analysis)
  * [Backup](#backup)
  * [Benchmarking](#benchmarking)
  * [Binlog Replication](#binlog-replication)
  * [ChatOps](#chatops)
  * [Configuration](#configuration)
  * [Connectors](#connectors)
  * [Deployment](#deployment)
  * [Development](#development)
  * [GUI](#gui)
  * [HA](#ha)
  * [MCP](#mcp)
  * [Proxy](#proxy)
  * [Replication](#replication)
  * [Schema](#schema)
  * [Security](#security)
  * [Server](#server)
  * [Sharding](#sharding)
  * [Toolkits](#toolkits)

* [Resources](#resources)
  * [E-Books](#e-books)

## Analysis

*Performance, structure & data analysis tools*

* [Prometheus](https://github.com/prometheus/prometheus) ⭐ 62,749 | 🐛 759 | 🌐 Go | 📅 2026-02-18/[mysqld\_exporter](https://github.com/prometheus/mysqld_exporter) ⭐ 2,404 | 🐛 184 | 🌐 Go | 📅 2026-02-16 - Time series database for real-time monitoring and alerting.
* [MySQLTuner-perl](https://github.com/major/MySQLTuner-perl) ⭐ 9,436 | 🐛 34 | 🌐 Perl | 📅 2026-02-14 - A script that allows you to review a MySQL installation quickly and make adjustments to increase performance and stability.
* [innodb-ruby](https://github.com/jeremycole/innodb_ruby) ⭐ 1,785 | 🐛 17 | 🌐 Ruby | 📅 2024-11-26 - A parser for InnoDB file formats, in Ruby.
* [Anemometer](https://github.com/box/Anemometer) ⭐ 1,396 | 🐛 60 | 🌐 JavaScript | 📅 2021-12-08 - Box SQL slow query monitor.
* [Dolphie](https://github.com/charles-001/dolphie) ⭐ 1,109 | 🐛 1 | 🌐 Python | 📅 2026-02-17 - a modern terminal tool for real-time analytics into MySQL/MariaDB & ProxySQL
* [sql-tap](https://github.com/mickamy/sql-tap) ⭐ 878 | 🐛 0 | 🌐 Go | 📅 2026-02-18 - Real-time SQL traffic viewer.
* [innotop](https://github.com/innotop/innotop) ⭐ 798 | 🐛 26 | 🌐 Perl | 📅 2025-10-22 - a 'top' clone for MySQL with many features and flexibility.
* [pstop](https://github.com/sjmudd/ps-top) ⭐ 210 | 🐛 6 | 🌐 Go | 📅 2026-02-10 - a top-like program for MySQL, collecting, aggregating and displaying information from performance\_schema.
* [mysql-statsd](https://github.com/db-art/mysql-statsd) ⭐ 102 | 🐛 6 | 🌐 Python | 📅 2021-04-20 - A Python daemon to collect information from MySQL and send it via StatsD to Graphite.
* [MySQL Explain Analyzer](https://github.com/Preetam/explain-analyzer) ⭐ 97 | 🐛 11 | 🌐 JavaScript | 📅 2023-03-06 - A web-based analyzer of `EXPLAIN FORMAT=JSON` output, providing comments, scalability analysis and permalinks for saved samples.
* [Wireshark](https://gitlab.com/wireshark/wireshark/) - a protocol analyzer that can decode the MySQL protocol.

## Backup

*Backup/restore/recovery tools*

* [Dumpling](https://github.com/pingcap/tidb/tree/master/dumpling) ⭐ 39,746 | 🐛 5,672 | 🌐 Go | 📅 2026-02-17 - Logical, parallel backup/dumper tool for MySQL/TiDB written in GoLang - support csv format output and integrated as library
* [Databasus](https://github.com/databasus/databasus) ⭐ 5,574 | 🐛 2 | 🌐 Go | 📅 2026-02-17 - tool for scheduled MySQL backups via web UI with external storages (local, S3, FTP, Google Drive, etc.), notifications (webhook, Discord, Slack, etc.) and team management.
* [MyDumper](https://github.com/mydumper/mydumper) ⭐ 3,028 | 🐛 49 | 🌐 C | 📅 2026-02-11 - Logical, parallel backup/dumper tool for MySQL
* [Percona Xtrabackup](https://github.com/percona/percona-xtrabackup) ⭐ 1,495 | 🐛 16 | 🌐 C++ | 📅 2026-01-29 - an open-source hot backup utility for MySQL - based servers that doesn’t lock your database during the backup.
* [Portabase](https://github.com/Portabase/portabase) ⭐ 322 | 🐛 8 | 🌐 TypeScript | 📅 2026-02-17 - Agent-based platform for MySQL backups and restores with decentralized execution and centralized orchestration.

## Benchmarking

*Tools to stress your servers*

* [Sysbench](https://github.com/akopytov/sysbench) ⭐ 6,677 | 🐛 213 | 🌐 C | 📅 2025-03-09 - a modular, cross-platform and multi-threaded benchmark tool.
* [HammerDB](https://github.com/TPC-Council/HammerDB) ⭐ 733 | 🐛 21 | 🌐 Tcl | 📅 2026-02-13 - An open-source database benchmark for MySQL/MariaDB and other open source and commercial databases.
* [TPCC-MySQL](https://github.com/Percona-Lab/tpcc-mysql) ⚠️ Archived (archived) - A port of the popular [TPCC](http://www.tpc.org/tpcc/) benchmark for MySQL.
* [go-tpc](https://github.com/pingcap/go-tpc) ⭐ 210 | 🐛 22 | 🌐 Go | 📅 2026-01-13 - A golang port of [TPCC](http://www.tpc.org/tpcc/) and [TPCH](http://www.tpc.org/tpch/) benchmark for MySQL.
* [iibench-mysql](https://github.com/tmcallaghan/iibench-mysql) ⭐ 46 | 🐛 3 | 🌐 Java | 📅 2017-12-04 - Java based version of the Index Insertion Benchmark for MySQL/Percona/MariaDB.

## Binlog-Replication

* [Kingbus](https://github.com/flike/kingbus) ⭐ 896 | 🐛 12 | 🌐 Go | 📅 2021-03-11 - A distributed MySQL binlog storage system built on Raft
* [DM](https://github.com/pingcap/tiflow) ⭐ 454 | 🐛 906 | 🌐 Go | 📅 2026-02-12 - A High-Availability data migration platform which supports migrating data from MySQL/MariaDB to TiDB and merging shard tables
* [mysql-ripple](https://github.com/google/mysql-ripple) ⚠️ Archived (archived) - Ripple, a server that can serve as a middleman in MySQL replication

## ChatOps

*Scripts integrated into chat rooms*

* [Hubot MySQL ChatOps](https://github.com/samlambert/hubot-mysql-chatops) ⭐ 90 | 🐛 0 | 🌐 CoffeeScript | 📅 2014-03-09

## Configuration

*MySQL sample configuration and advisors*

* [mysql-compatibility-config](https://github.com/morgo/mysql-compatibility-config) ⭐ 94 | 🐛 1 | 🌐 Shell | 📅 2017-03-02 - make MySQL configuration behave more like newer (or older) releases of MySQL.

## Connectors

*MySQL connectors for various programming languages*

* [node-mysql](https://github.com/mysqljs/mysql) ⭐ 18,842 | 🐛 172 | 🌐 JavaScript | 📅 2024-06-25 - A pure Nodejs Javascript client implementing the MySQL protocol.
* [go-sql-driver](https://github.com/go-sql-driver/mysql) ⭐ 15,422 | 🐛 73 | 🌐 Go | 📅 2025-06-13 - a lightweight and fast MySQL-Driver for Go's (golang) database/sql package.
* [PyMySQL](https://github.com/PyMySQL/PyMySQL) ⭐ 7,841 | 🐛 24 | 🌐 Python | 📅 2025-08-24 - MySQL database connector for Python.
* [mysqlclient-python](https://github.com/PyMySQL/mysqlclient) ⭐ 2,524 | 🐛 9 | 🌐 Python | 📅 2026-02-12 - MySQL database connector for Python.
* [Ruby Mysql2 gem](https://github.com/brianmario/mysql2) ⭐ 2,279 | 🐛 197 | 🌐 Ruby | 📅 2025-10-22 - MySQL driver for Ruby and Rails projects.
* [MySQL Connector/J](https://github.com/mysql/mysql-connector-j) ⭐ 1,009 | 🐛 1 | 🌐 Java | 📅 2026-01-22 - a standardized database driver for the Java platforms and development.
* [MySQL Connector/Python](https://github.com/mysql/mysql-connector-python) ⭐ 943 | 🐛 1 | 🌐 Python | 📅 2026-02-10 - a standardized database driver for Python platforms and development.
* [MySQL Connector/C++](https://github.com/mysql/mysql-connector-cpp) ⭐ 701 | 🐛 0 | 🌐 C++ | 📅 2026-01-21 - Official C/C++ driver for MySQL.
* [MariaDB Connector/J](https://github.com/mariadb-corporation/mariadb-connector-j) ⭐ 357 | 🐛 5 | 🌐 Java | 📅 2026-02-17 - LGPL-licensed MariaDB Client Library for Java Applications.
* [wtx](https://github.com/c410-f3r/wtx) ⭐ 342 | 🐛 12 | 🌐 Rust | 📅 2026-02-11 - Client for MySQL/MariaDB/Percona written in Rust
* [MySQL Connector/NET](https://github.com/mysql/mysql-connector-net) ⭐ 324 | 🐛 0 | 🌐 C# | 📅 2026-01-21 - a standardized database driver for .Net platforms and development.
* [MySQL Connector/Node.js](https://github.com/mysql/mysql-connector-nodejs) ⭐ 159 | 🐛 0 | 🌐 JavaScript | 📅 2024-10-22 - Official Node.js driver for MySQL.
* [ballerinax/mysql](https://github.com/ballerina-platform/module-ballerinax-mysql) ⭐ 111 | 🐛 5 | 🌐 Ballerina | 📅 2026-02-16 - Official Ballerina connector for MySQL.
* [MyZql](https://github.com/speed2exe/myzql) ⭐ 67 | 🐛 5 | 🌐 Zig | 📅 2025-11-21 - MySQL and MariaDB driver in native Zig.
* [DBD::mysql](https://github.com/perl5-dbi/DBD-mysql) ⭐ 66 | 🐛 72 | 🌐 Perl | 📅 2026-02-01 - MySQL driver for the Perl5 Database Interface.
* [DBD::MariaDB](https://github.com/perl5-dbi/DBD-MariaDB) ⭐ 40 | 🐛 20 | 🌐 Perl | 📅 2025-05-04 - MariaDB and MySQL driver for the Perl5 Database Interface.
* [libAttachSQL](https://github.com/libattachsql/libattachsql) ⭐ 29 | 🐛 24 | 🌐 C++ | 📅 2020-08-28 - libAttachSQL is a lightweight, non-blocking C API for MySQL servers.
* [mex-mariadb](https://github.com/markuman/mex-mariadb) ⭐ 2 | 🐛 1 | 🌐 C | 📅 2022-11-04 - MIT licensed MariaDB/MySQL Client Library for GNU Octave and Matlab.
* [MySQL C API](https://dev.mysql.com/downloads/c-api/) - Official C driver for MySQL.
* [PHP mysqlnd](https://www.php.net/manual/en/book.mysqlnd.php) - MySQL native driver for PHP.

## Deployment

*MySQL deployment tools*

* [MariaDB4j](https://github.com/MariaDB4j/MariaDB4j) ⭐ 895 | 🐛 4 | 🌐 Java | 📅 2026-01-02 - A Java launcher to run MariaDB without installation or external dependencies.

## Development

*Tools to support MySQL-related development*

* [Flywaydb](https://github.com/flyway/flyway) ⭐ 9,539 | 🐛 241 | 🌐 Java | 📅 2026-02-12 - Database migrations; Evolve your database schema easily and reliably across all your instances
* [Liquibase](https://github.com/liquibase/liquibase) ⭐ 5,426 | 🐛 685 | 🌐 Java | 📅 2026-02-17 - Source control for your database
* [Test database](https://github.com/datacharmer/test_db) ⭐ 4,387 | 🐛 0 | 🌐 Shell | 📅 2026-02-13 - A sample MySQL database with an integrated test suite, used to test applications and servers
* [SQLE](https://github.com/actiontech/sqle/blob/main/README_en.md) ⭐ 1,472 | 🐛 170 | 🌐 Go | 📅 2026-02-06 - SQLE is a SQL audit platform for DBA or developer
* [Skeema](https://github.com/skeema/skeema) ⭐ 1,358 | 🐛 16 | 🌐 Go | 📅 2026-02-13 - Declarative pure-SQL schema management system for MySQL and MariaDB, with support for sharding and external online schema change tools
* [Shift](https://github.com/square/shift) ⭐ 741 | 🐛 29 | 🌐 Ruby | 📅 2025-04-01 - An application that helps you run schema migrations on MySQL databases

## GUI

*GUI frontends & applications*

* [DBeaver](https://github.com/dbeaver/dbeaver/) ⭐ 48,709 | 🐛 3,228 | 🌐 Java | 📅 2026-02-18 - A cross-platform SQL and NoSQL database client.
* [ILLA Cloud](https://github.com/illacloud/illa-builder) ⭐ 12,373 | 🐛 43 | 🌐 TypeScript | 📅 2026-02-15 - Low-code internal tool builder integrated with Mysql, can be used as GUI for Mysql.
* [mycli](https://github.com/dbcli/mycli) ⭐ 11,870 | 🐛 15 | 🌐 Python | 📅 2026-02-17 - A Terminal Client for MySQL with AutoCompletion and Syntax Highlighting.
* [phpMyAdmin](https://github.com/phpmyadmin/phpmyadmin) ⭐ 7,797 | 🐛 913 | 🌐 PHP | 📅 2026-02-17 - a free software tool written in PHP, intended to handle the administration of MySQL over the Web.
* [Sequel Ace](https://github.com/Sequel-Ace/Sequel-Ace) ⭐ 7,298 | 🐛 233 | 🌐 Objective-C | 📅 2026-02-12 - a Mac database management application for working with MySQL databases.
* [Adminer](https://github.com/vrana/adminer/) ⭐ 7,268 | 🐛 23 | 🌐 PHP | 📅 2026-02-12 - Database management in a single PHP file.
* [HeidiSQL](https://github.com/HeidiSQL/HeidiSQL) ⭐ 5,806 | 🐛 419 | 🌐 Pascal | 📅 2026-02-17 - MySQL GUI frontend for Windows.
* [OmniDB: Web tool for database management](https://github.com/OmniDB/OmniDB) ⭐ 3,276 | 🐛 329 | 🌐 JavaScript | 📅 2023-02-01
* [pspg](https://github.com/okbob/pspg) ⭐ 2,689 | 🐛 1 | 🌐 C | 📅 2026-02-15 - provides a pager with enhanced visualization and navigation for tabular data. Originally implemented for PostgreSQL, but also supports MySQL.
* [SQLyog Community edition](https://github.com/webyog/sqlyog-community) ⭐ 2,322 | 🐛 689 | 🌐 C++ | 📅 2025-10-03 - SQLyog Community edition. For Windows, works fine under wine in Mac and Linux
* [MySQL Workbench](https://github.com/mysql/mysql-workbench) ⭐ 983 | 🐛 1 | 🌐 C++ | 📅 2026-01-21 - provides DBAs and developers an integrated tools environment for database design & modeling; SQL devleopment; database administration.
* [Percona Monitoring and Management](https://github.com/percona/pmm) ⭐ 965 | 🐛 176 | 🌐 Go | 📅 2026-02-18 - An open-source platform for managing and monitoring MySQL performance.
* [WebDB](https://github.com/WebDB-App/app) ⭐ 333 | 🐛 25 | 🌐 TypeScript | 📅 2025-06-10 – Open Source and Efficient Database IDE. Featuring Easy server connection, Modern ERD, Intelligent data generator, AI assistant, NoSQL structure manager, Time machine and Powerful query editor
* [MySQL Shell](https://github.com/mysql/mysql-shell/) ⭐ 217 | 🐛 0 | 🌐 C++ | 📅 2026-01-20 - Advanced client and code editor for MySQL that supports development and administration for the MySQL Server and MySQL InnoDB cluster (AdminAPI) with an interactive JavaScript, Python, or SQL interface.
* [Ocelot GUI](https://github.com/ocelot-inc/ocelotgui) ⭐ 63 | 🐛 2 | 🌐 C++ | 📅 2025-11-06 - GUI client for MySQL or MariaDB, including debugger.

## HA

*High availability solutions*

* [Orchestrator](https://github.com/openark/orchestrator) ⚠️ Archived (archived) - MySQL replication topology management and High Availability solution.
* [replication-manager](https://github.com/signal18/replication-manager) ⭐ 726 | 🐛 143 | 🌐 Go | 📅 2026-02-16 - a high availability solution to manage MariaDB 10.x and MySQL & Percona Server 5.7 GTID replication topologies.
* [Galera Cluster](https://github.com/codership/galera) ⭐ 485 | 🐛 248 | 🌐 C++ | 📅 2025-10-06 - a true Multimaster Cluster based on synchronous replication.
* [mha4mysql-node](https://github.com/yoshinorim/mha4mysql-node) ⭐ 410 | 🐛 14 | 🌐 Perl | 📅 2020-03-12 and [mha4mysql-manager](https://github.com/yoshinorim/mha4mysql-manager) ⭐ 1,519 | 🐛 73 | 🌐 Perl | 📅 2020-08-14 (both unmaintained) - Master High Availability Manager and tools for MySQL.
* [Percona Replication Manager](https://github.com/percona/replication-manager) ⭐ 7 | 🐛 2 | 🌐 Shell | 📅 2026-01-07 - Asynchronous MySQL replication manager agent for Pacemaker. Supports file and GTID based replication, geo-distributed clusters using booth.

## MCP

* [MCP MariaDB Server](https://github.com/MariaDB/mcp) ⭐ 130 | 🐛 18 | 🌐 Python | 📅 2026-01-05 - the official MariaDB MCP server.
* [MySQL MCP Server](https://github.com/askdba/mysql-mcp-server) ⭐ 9 | 🐛 6 | 🌐 Go | 📅 2026-02-10 - Advanced MCP server exposing MySQL via the Model Context Protocol
* [TiDB MCP Server](https://pingcap.github.io/ai/integrations/tidb-mcp-server/) - MCP Server for TiDB.

## Proxy

*Proxies to MySQL*

* [MySQL Router](https://dev.mysql.com/doc/mysql-router/en/) - MySQL Router is part of InnoDB cluster, and is a lightweight middleware that provides transparent routing between your application and back-end MySQL Servers.
* [ProxySQL](https://github.com/sysown/proxysql) ⭐ 6,624 | 🐛 1,107 | 🌐 C++ | 📅 2026-02-18 - High performance proxy for MySQL.

## Replication

*Replication related software*

* [data-diff](https://github.com/datafold/data-diff) ⚠️ Archived (archived) - Command-line tool and Python library to efficiently diff rows across two different databases.

## Schema

*Add-on schemas*

* [sys](https://github.com/mysql/mysql-sys) ⚠️ Archived (archived) - A collection of views, functions and procedures to help MySQL administrators get insight in to MySQL Database usage. See [sys schema docs](https://dev.mysql.com/doc/refman/8.4/en/sys-schema.html)
* [common\_schema](https://github.com/shlomi-noach/common_schema) ⭐ 126 | 🐛 17 | 🌐 PLpgSQL | 📅 2020-03-21 - DBA's framework for MySQL, providing a function library, views library and QueryScript interpreter.

## Security

*Tools that prevents leaking of sensitive data from database (encryption, masking and tokenization, honey-pots, etc)*

* [Acra](https://github.com/cossacklabs/acra) ⭐ 1,453 | 🐛 16 | 🌐 Go | 📅 2025-12-05 - SQL database protection suite: strong selective encryption, SQL injections prevention, intrusion detection system.
* [myanon](https://github.com/ppomes/myanon) ⭐ 114 | 🐛 0 | 🌐 C | 📅 2026-02-17 - Streaming anonymizer for MySQL dump files, reading mysqldump output from stdin and writing anonymized data to stdout. Supports deterministic hashing, fixed values, JSON field anonymization, and Python extensions.
* [myldapsync](https://github.com/6eh01der/myldapsync) ⭐ 0 | 🐛 0 | 🌐 Python | 📅 2025-10-19 - Synchronize MySQL or MariaDB users with users in an LDAP directory.

## Server

*MySQL server flavors*

* [TiDB](https://github.com/pingcap/tidb) ⭐ 39,746 | 🐛 5,672 | 🌐 Go | 📅 2026-02-17 - A distributed HTAP database compatible with the MySQL protocol.
* [MySQL Server & MySQL Cluster](https://github.com/mysql/mysql-server) ⭐ 12,082 | 🐛 1 | 🌐 C++ | 📅 2026-01-22 - Official Oracle's MySQL server & MySQL Cluster distribution.
* [MariaDB](https://github.com/MariaDB/server) ⭐ 7,187 | 🐛 277 | 🌐 C++ | 📅 2026-02-17 - Community developed fork of MySQL server.
* [Percona Server](https://github.com/percona/percona-server) ⭐ 1,254 | 🐛 59 | 🌐 C++ | 📅 2026-02-17 - An enhanced, drop-in MySQL replacement.
* [MyVector](https://github.com/askdba/myvector) ⭐ 1 | 🐛 3 | 🌐 C++ | 📅 2026-02-12 - Native vector search plugin for MySQL, shipped as a server plugin.

## Sharding

*Sharding solutions/frameworks*

* [Vitess](https://github.com/vitessio/vitess) ⭐ 20,701 | 🐛 925 | 🌐 Go | 📅 2026-02-18 - vitess provides servers and tools which facilitate scaling of MySQL databases for large scale web services.
* [Jetpants](https://github.com/tumblr/jetpants) ⭐ 1,128 | 🐛 3 | 🌐 Ruby | 📅 2017-06-15 - An automation suite for managing large range sharding clusters, by Tumblr.

## Toolkits

*Toolkits, general purpose scripts*

* [gh-ost](https://github.com/github/gh-ost/) ⭐ 13,215 | 🐛 322 | 🌐 Go | 📅 2026-02-10 - GitHub's online schema migration for MySQL.
* [go-mysql](https://github.com/go-mysql-org/go-mysql) ⭐ 4,920 | 🐛 152 | 🌐 Go | 📅 2026-02-18 - A pure go library to handle MySQL network protocol and replication.
* [Percona Toolkit](https://github.com/percona/percona-toolkit) ⭐ 1,449 | 🐛 26 | 🌐 Perl | 📅 2026-02-17 - a collection of advanced command-line tools to perform a variety of MySQL server and system tasks that are too difficult or complex to perform manually.
* [UnDROP](https://github.com/twindb/undrop-for-innodb) ⚠️ Archived (archived) - a tool to recover data from dropped or corrupted InnoDB tables.
* [MySQL Utilities](https://github.com/mysql/mysql-utilities) ⚠️ Archived (deprecated) - a collection of command-line utilities, written in Python, that are used for maintaining and administering MySQL servers, either individually, or within Replication hierarchies.
* [Swoof](https://github.com/StirlingMarketingGroup/swoof) ⭐ 28 | 🐛 0 | 🌐 Go | 📅 2026-01-12 - Ultra fast MySQL table importer that stages swaps through temporary tables and supports file/clipboard targets.
* [sql-splitter](https://github.com/HelgeSverre/sql-splitter) ⭐ 3 | 🐛 0 | 🌐 Rust | 📅 2026-02-17 - High-performance CLI for splitting, merging, converting, validating, and sampling mysqldump files.

# Resources

*At this stage "resources" will not include websites, blogs, slides, presentation videos, etc. in fear of list size*

## e-books

*e-books as well as relevant materials on and around MySQL*

* [Database Systems Lecture Notes](http://spots.augusta.edu/caubert/db/ln/) - lecture notes on Database Systems (available in pdf, html, odt and markdown) including a Chapter on SQL that covers basic set-up, exercises and problems.
* [SQL-exercise](https://github.com/XD-DENG/SQL-exercise) ⭐ 1,477 | 🐛 8 | 📅 2023-11-11 - contains several SQL exercises, including the schema description figure, SQL code to build schema, questions and solutions in SQL. Based on wikibook [SQL Exercises](https://en.wikibooks.org/wiki/SQL_Exercises).

## Incubating

Projects that are known to be non-production and yet have either traction or substance that warrants exposure.

* [VillageSQL](https://github.com/villagesql/villagesql-server) ⭐ 89 | 🐛 15 | 🌐 C++ | 📅 2026-02-17 - A drop-in replacement for MySQL with extensions for the agentic AI era.
