# Hosting and querying a PostgreSQL database

[ElephantSQL](https://www.elephantsql.com/) is useful for free hosting. Try [Heroku](https://www.heroku.com/pricing#databases) too.

Switch from *Details* to *browser* and you can run SQL queries there.

You can however use [Mode](https://modeanalytics.com/) to connect to the database and query it (and export the resulting reports). Note that the username and the name of the database are the same. 

Mode has [tutorials on SQL](https://community.modeanalytics.com/sql/tutorial/introduction-to-sql/)

In my case the default database was called

To find the name of the database, go to the Mode homepage and then click on your data source in the left column - specifically the three dots next to it, and select **Settings**. The name of your table should be in there. Here's an example query if the table is called `public.pg_stat_statements`:

`select * from public.pg_stat_statements where calls > 100`

## Other tools

[From the ElephantSQL documentation](https://www.elephantsql.com/docs/index.html)

> "[psql](https://www.postgresql.org/docs/9.1/static/app-psql.html) is an interactive terminal for work with Postgres and [pgAdmin](https://www.elephantsql.com/docs/pgadmin.html) is a graphical administration client for PostgreSQL. 
