- Pull current existing database with `npx prisma db pull`, you can clear all current schemas and leave only `generator` and `datasource`
- Delete existing table `_prisma_migrations`
- Export current DB without re-creating tables, which mean we only export the data
- Delete `prisma/migrations` folder
- Create a new migration with `npx prisma migrate dev --name initial_migration`
- After tables successfully created, we need to import previously exported database data to current version of database
- Make sure `_prisma_migrations` didn't bring data from previous database
- Finish~
