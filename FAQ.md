cacti-sqlite FAQ
============


Installation
------------

1. Installed Debian on Raspi Pi
2. installed php, php-sqlite, sqlite3, snmpd, snmp
3. Downloaded from Github the cacti files an stored them in /var/www/cacti
4. Created a Database in /var/lib/sqlite/cacti.db an run the sql-script ( the tables would be created)
```sh
sqlite3 /path/to/cacti.db < cacti-sqlite.sql
```

5. entered the path entry in include/config.php ($database_port = "/var/lib/sqlite/cacti.db";)
6. configure web server
7. Run <ip>/cacti and follow the usual cacti installation process.


Howto
------------
Q1.
PHP Fatal error: pdo error: [-1: Connection attempt failed: could not find driver] in CONNECT(sqlite:/var/lib/sqlite/cacti.db, '****', '****', )\n in /var/www/cacti/lib/adodb/adodb-errorhandler.inc.php on line 77

A1.
1. check whether php-sqlite3 installed
2. check cacti.db ownship and group ,MUST have right to write for web server( user/group www-data for nginx)
