# Docker scaffold
this is a basic scaffold i have made so that i won't have to deal with the headache of dealing with setting up a docker environment all over again for development of future web apps. 

It prepares 4 containers

assuming you have the docker environment installed along with docker-compose  
- **php**  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a container that hosts the php executable and app itself  
- **mysql**  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the container that hosts the database  
-  **phpmyadmin**  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the container that hosts phpmyadmin so you can access the mysql database  
-  **nginx**  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;the webserver

just run the following from the command line and you are ready to go  
```bash
docker-compose up
```

the actual code of your project goes into the ./app folder

Depending on the needs of your project you might have to make some changes to the docker-compose.yml
especially the MYSQl_ROOT_PASSWORD, the MYSQL_DATABASE, as well as the MYSQL_USER and MYSQL_PASSWORD

until i figure out a way to make some kind of script to change these for you, it will have to be done manually.

