## MySQL role

Some description for MySQL role would be nice. Any volunteers?

### Parameters

**mysql_version** (type `string`, default `5.7.*`)

Example:
```yaml
mysql_version: 5.6.*
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