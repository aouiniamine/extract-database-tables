
# extract database tables

## I. init env
#### 1.
```bash 
npm install
```

#### 2. add DATABASE_URL to .env file

#### 3. change provider to myqsl if needed in prisma/schema.prisma


## II. extract sql tables

```bash
npx prisma migrate diff --from-empty --to-schema-datasource prisma/schema.prisma --script > db_tables.sql
```
