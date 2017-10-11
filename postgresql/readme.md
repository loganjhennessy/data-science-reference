# Installation

The postgres [setup guide](http://postgresguide.com/setup/install.html)
specifies the following line to use to install postgresql.

```bash
sudo apt-get install postgresql
```

# Adding a User

Remember that, at first, the only user that exists to postgresql is
`postgresql`. So you'll need to execute the following command to set
user to `postgresql`:

```bash
sudo su postgresql
```

Once that has  executed successfully, the standard `psql` command will
work.

At that point, you need to create a new user within psql and grant them
privileges. This can be done with the following commands:

```bash
CREATE USER <username> WITH PASSWORD '<password>';
```

Assuming that the username matches your system user name, this will
allow you to access the `psql` prompt without having to `su` to
`postgresql`.

# Creating the database

This is a pretty simple one:

```bash
CREATE DATABASE <dbname>;
```

# Creating tables
