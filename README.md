# Microblogging App!

## To install on your VM

1. Clone the app into your shared folder `git clone git@github.com:DCSIL-summer-course/rails-app.git`
2. Run:

```bash
rake db:setup
rake db:migrate
```

## Errors

If you already have a database with the same name that `rails-app` uses you'll like get errors. To delete the existing database in your VM do the following:

```
sudo su postgres
psql
```

then, once psql has loaded:

```sql
DROP DATABASE twitterclone_development;
DROP DATABASE twitterclone_test;
```

The run the `rake` commands again.
