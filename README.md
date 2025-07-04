
##  Database Backup Utility

A database backup utility that can backup and restore any DB. 

### Previous to use the tool 

Please ensure that the binaries for the database you wish to dump or restore are installed. If you already have a server running, verify that the binaries are included in your system's PATH.

[PostgreSQL](https://www.postgresql.org/download/)

[MySQL Community Edition](https://www.mysql.com/products/community/)

[MongoDB Tools](https://www.mongodb.com/try/download/database-tools)

### How to install

Make sure you have installed [Node.js](https://nodejs.org/en)

Open a command line: 

```
git clone https://github.com/tholliver/db-backup-utility.git

cd db-backup-utility

npm install 
```

## How to use

###  Backup Examples: 

For PostgreSQL:

```
node cli backup -db postgresql -h localhost --user pguser --password secretPass --port 5433 --database DummyDatabase
```

For MySQL:

```
node cli backup -db mysql -h localhost -u root -pw secretPass -p 3306 -d DummyDatabase
```

For MongoDB:

```
node cli backup -db mongodb -h localhost -u admin -pw secretPass -d DummyDatabase
```

**Currently, the backup files are saved in the project's directory, inside the [backups] folder.**

###  Restore Examples: 

*FEATURE NOT AVAIABLE YET*

For more details: 

```
node cli -h

node cli backup --help
```

#### Supported databases (Backup)

- MySQL 
- PostgreSQL
- MongoDB


### Future Features/Upcoming Features

#### Mains
- Backup Types
- Compression
- Cloud Storage
- Logging and Notifications
- Restore Operations (Selective Restore/Restore Backup) 

### Maybes
- JSON credentials reader
- Custom backup DIR  

