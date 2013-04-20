cacti-sqlite
============

Cacti SQLite

The original work was published by beagle1 on Cacti Forums (http://forums.cacti.net/viewtopic.php?f=21&t=48177), all the merit goes to him/her. Finding it difficult to share patches I created this repository. Fork, patch, improve and enjoy.


Installation
------------

```sh
sqlite3 /path/to/db < cacti-sqlite.sql
```
configure include/config.php with the proper db path and follow the usual cacti configuration.