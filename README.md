cacti-sqlite
============

Cacti SQLite

The original work was published by beagle1 on Cacti Forums (http://forums.cacti.net/viewtopic.php?f=21&t=48177), all the merit goes to him/her. Finding it difficult to share patches I created this repository. Fork, patch, improve and enjoy.

Cacti (http://cacti.net/) is a complete network graphing solution designed to harness the power of RRDTool's data storage and graphing functionality. Cacti provides a fast poller, advanced graph templating, multiple data acquisition methods, and user management features out of the box. All of this is wrapped in an intuitive, easy to use interface that makes sense for LAN-sized installations up to complex networks with hundreds of devices.

This fork allows you to run Cacti on SQLite instead of MySQL making it easier to run it on limited resources machines (i.e. Raspberry Pi).

Installation
------------

```sh
sqlite3 /path/to/db < cacti-sqlite.sql
```
configure include/config.php with the proper db path and follow the usual cacti installation process.