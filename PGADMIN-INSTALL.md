

 # install postgres - kali
 [install on kai-linux](https://www.postgresql.r2schools.com/how-to-install-postgresql-on-kali-linux/)

 [postgres docs](https://www.postgresql.org/download/linux/debian/)


```
sudo apt-get install wget ca-certificates
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main" >> /etc/apt/sources.list.d/pgdg.list'
sudo apt-get update
sudo apt-get install postgresql postgresql-contrib

```

```
sudo su - postgres
psql
```

# install pgadmin
[pgadmin4 install kali](https://www.geeksforgeeks.org/how-to-install-pgadmin4-in-kali-linux/)
```
sudo curl https://www.pgadmin.org/static/packages_pgadmin_org.pub | sudo apt-key add

sudo sh -c 'echo "deb https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/bullseye/ pgadmin4 main" > /etc/apt/sources.list.d/pgadmin4.list && apt update'

# for both desktop & web
sudo apt install pgadmin4

# configure we server
#sudo /usr/pgadmin4/bin/setup-web.sh


```