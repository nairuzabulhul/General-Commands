
![Log](https://s31.postimg.org/sr1qvkkp7/mongo.png)

# Install mongodb in Cloud9

1- Create a new directory with name data 

>>``` mkdir data```

2- Install mongodb:

>> ```sudo apt-get install mongodb-org```

3- Setup the Path 

``` echo 'mongod --bind_ip=$IP --dbpath=data --nojournal --rest "$@"' > mongod ```


4- Make mongod exectutable 

``` chmod a+x mongod ```

5- Run monogo

>> ```./mongo ```


6- Start mongo (other option)

```sudo service mongod start```

7- Stop monog

```sudo service mongod stop ```

8- Restart mongo

```sudo service mongod restart ```

9- Remove packages:

```sudo apt-get purge mongodb-org*```

10- Remove Data Directories

```sudo rm -r /var/log/mongodb ```

```sudo rm -r /var/lib/mongodb   ```


##Interactign with monogdb:


1- run database:

>> type monog in the terminal and the shell will come up 


2- Show all database:

```show dbs ```

3- Select a database:

``` use nameOfYourDB ```

4- Show the items in the database:

``` show collections ```

5- To Show all data in one database

``` db.nameOFDB.find() ```
