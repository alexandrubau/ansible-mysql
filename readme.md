## MySQL role

Some description for MySQL role would be nice. Any volunteers?  
We use MariaDb.

### Parameters

**mysql_version** (type `string`, default `10.0.*`)

Example:
```yaml
mysql_version: 10.0.*
```

**mysql_databases** (type `array`, default `[]`)

Example:
```yaml
mysql_databases:
 - projectdb
```

**mysql_users** (type `array`, default `[]`)

Example:
```yaml
mysql_users:
 - username: 'athena'
   password: 'athena'
   privs:
     - '*.*:ALL,GRANT'
   hosts:
     - '%'
     - 'localhost'
```