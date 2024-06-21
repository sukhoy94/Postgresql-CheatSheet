# Postgresql-CheatSheet

## Indexes

### 1. Creating an index
```
CREATE INDEX IF NOT EXISTS index_name
  ON schema.table_name USING btree
  (column1_name1 ASC NULLS LAST, column2_name ASC NULLS LAST, ...)
  TABLESPACE pg_default;
```
### 2. Delete an index
```
DROP INDEX IF EXISTS schema.index_name;
```
