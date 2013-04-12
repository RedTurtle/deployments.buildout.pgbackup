deployments.buildout.pgbackup
=============================

A buildout template for backing up postgresql

For the impatients
------------------
Those are the commands you want to run
```
sudo chown -R postgres. .
sudo su postgres
virtualenv-2.7 --no-site-packages -p /usr/bin/python2.7 .
. bin activate
ln -s config/base.cfg buildout.cfg
./bin/python2.7 bootstrap.py
./bin/buildout
./bin/backup
```

Configuritations and options
----------------------------
Take a look in the comments of `config/base.cfg`

TODO
----
Restore script.
