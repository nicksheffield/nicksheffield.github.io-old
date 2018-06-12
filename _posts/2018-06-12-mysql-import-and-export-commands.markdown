---
title:  "Mysql import and export commands"
---

### To import

```
mysql -u username -p databasename < db_backup.sql
```

### To export

```
mysqldump -u username -p databasename > db_backup.sql
```

### To clear

```
mysql -u username -p -e "USE databasename; DROP TABLE IF EXISTS table1, table2, table3, etc;"
```
