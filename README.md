# linux-webserver
This contains the information and details to login to the linux server for full stack nanodegree course exam.

How to login
----

1. Please use the key to login to the server
2. store the key in `~/.ssh/grader_key`
3. Then ssh and login to the server - `18.197.62.160` ip address and `grader` is the user with sudo
4. hostname for the server - `catalogitems.sytes.net`
```sh
ssh grader@catalogitems.sytes.net -p 2200 -i ~/.ssh/grader_key
```
4. The website is hosted - [item-catalog](http://catalogitems.sytes.net/)

Softwares installed
----

1. nginx
2. uwsgi
3. Python3
4. Database - POSTGRESql

Resources used
----
1. Configurations made as detailed in [Digitalocean](https://www.digitalocean.com/community/tutorials/how-to-serve-flask-applications-with-uwsgi-and-nginx-on-ubuntu-16-04)

Configurations
-----
1. The DB `Postgres` is listening to port 5432 and can be accessed using `psql`
2. DB details
  * DBNAME - postgres
  * DBUSER - postgres
  * DBPASSWORD - postgres
2. `nginx` is configured to host `catalogitems.sytes.net`, the config file is in `/etc/nginx/sites-available/item-catalog`
3. `SSH` is configured to use port 2200 to signing
3. `ufw` was used to configure to allow access from server to outside, but only ports `80`, `2200` and `123` can be accessed from outside

License
----

MIT
