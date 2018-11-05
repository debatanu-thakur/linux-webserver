# linux-webserver
This contains the information and details to login to the linux server for full stack nanodegree course exam.

How to login
----

1. Please use the key to login to the server
2. store the key in `~/.ssh/grader_key`
3. Then ssh and login to the server - `18.197.62.160` ip address and `grader` is the user with sudo
```sh
ssh grader@18.197.62.160 -p 2200 -i ~/.ssh/grader_key
```
4. The website is hosted - [item-catalog](http://18.197.62.160/)

Softwares installed
----

1. nginx
2. uwsgi
3. Configurations made as detailed in [Digitalocean](https://www.digitalocean.com/community/tutorials/how-to-serve-flask-applications-with-uwsgi-and-nginx-on-ubuntu-16-04)

License
----

MIT
