# PostgreSQL




## Convert query into CSV

### Copy command

```
COPY (<auery>) To '/tmp/test.csv' With CSV DELIMITER ',';
```

example

```
COPY (Select * From foo) To '/tmp/test.csv' With CSV DELIMITER ',';
```

### psql cli
```
psql -d dbname -t -A -F"," -c "select * from users" > output.csv
```
