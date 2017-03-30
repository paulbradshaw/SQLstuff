# Hosting and querying a PostgreSQL database

[ElephantSQL](https://www.elephantsql.com/) is useful for free hosting. Try [Heroku](https://www.heroku.com/pricing#databases) too.

You can then use [Mode](https://modeanalytics.com/) to connect to the database and query it. Note that the username and the name of the database are the same. 

Mode has [tutorials on SQL](https://community.modeanalytics.com/sql/tutorial/introduction-to-sql/)

In my case the default database was called

To find the name of the database, go to the Mode homepage and then click on your data source in the left column - specifically the three dots next to it, and select **Settings**. The name of your table should be in there. Here's an example query if the table is called `public.pg_stat_statements`:

`select * from public.pg_stat_statements where calls > 100`
