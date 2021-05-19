<h1 align="center">Welcome to Migration-Tutorials 👋</h1>
<p>
</p>

> Migrating from SQLite to MariaDB

## Install

```sh
pip install sqlite3mysql
```

## Usage

```sh
install python/python3 to use this command
```
```sh
sqlite3mysql --sqlite-file database.db -X -p -h host -P port -S -u user -d schema
```
```sh
Please make sure to use all of this flags in the command for make it work properly.
--sqlite-file - your sqlite database.db / database.sqlite3 file
-X - Do not transfer foreign keys
-h host
-P - port
-S - Skip SSL
-u - user
-d schema
```
#All module options
``sh
Usage: sqlite3mysql [OPTIONS]

  Transfer SQLite to MySQL using the provided CLI options.

Options:
  -f, --sqlite-file PATH       SQLite3 database file  [required]
  -t, --sqlite-tables TEXT     Transfer only these specific tables (space
                               separated table names). Implies --without-
                               foreign-keys which inhibits the transfer of
                               foreign keys.

  -X, --without-foreign-keys   Do not transfer foreign keys.
  -d, --mysql-database TEXT    MySQL database name  [required]
  -u, --mysql-user TEXT        MySQL user  [required]
  -p, --prompt-mysql-password  Prompt for MySQL password
  --mysql-password TEXT        MySQL password
  -h, --mysql-host TEXT        MySQL host. Defaults to localhost.
  -P, --mysql-port INTEGER     MySQL port. Defaults to 3306.
  -S, --skip-ssl               Disable MySQL connection encryption.
  --mysql-integer-type TEXT    MySQL default integer field type. Defaults to
                               INT(11).

  --mysql-string-type TEXT     MySQL default string field type. Defaults to
                               VARCHAR(255).

  -T, --use-fulltext           Use FULLTEXT indexes on TEXT columns. Will
                               throw an error if your MySQL version does not
                               support InnoDB FULLTEXT indexes!

  --with-rowid                 Transfer rowid columns.
  -c, --chunk INTEGER          Chunk reading/writing SQL records
  -l, --log-file PATH          Log file
  -q, --quiet                  Quiet. Display only errors.
  --version                    Show the version and exit.
  --help                       Show this message and exit.
```



## Author

👤 **InSelfControll**

* Github: [@InSelfControll](https://github.com/InSelfControll)

## Show your support

Give a ⭐️ if this project helped you!

***
_This README was generated with ❤️ by [InSelfControll](https://github.com/kefranabg/readme-md-generator)_
# Migration-Tutorials
