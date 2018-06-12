---
title:  "Mysql import and export commands"
---

# To import

```
mysql -u username -p databasename < db_backup.sql
```

# To export

```bash
mysqldump -u username -p databasename > db_backup.sql
```
