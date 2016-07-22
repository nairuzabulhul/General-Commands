
![Log](https://s31.postimg.org/sr1qvkkp7/mongo.png)

# Install mongodb in Cloud9

1- Create a new directory with name data 

>>``` mkdir data```

2- Install mongodb:

>> ```sudo apt-get install mongodb-org```


3- Run monogo

>> ```./mongo ```


4- Start mongo (other option)

```sudo service mongod start```

5- Stop monog

```sudo service mongod stop ```

6- Restart mongo

```sudo service mongod restart ```

7- Remove packages:

```sudo apt-get purge mongodb-org*```

8- Remove Data Directories

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
