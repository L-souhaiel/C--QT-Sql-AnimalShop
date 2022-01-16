# Animal Shop Desktop App C++ Qt SQL

A C++ Desktop Application To manipulate buy and sell of  Animal  using QT library and  SQL Relational Data Base.

![Layout](https://github.com/TitiLouati/C--QT-Sql-AnimalShop/blob/main/AnimalShop.png)

# Example

Assuming That the Database is Already connected to the Application and everything is installed . After executing the App the user can : 


```

choose to sign up / in or to sign as a guest. 

choose Admin mode where user can see profit gain or choose to add or to delete an Animal .

choose Normal mode where user can  select the search criteria like which Spicies of Animal , maximal prices , Color , Date of birth and then buy An Animal from given Table.


```

![Layout2](https://github.com/TitiLouati/C--QT-Sql-AnimalShop/blob/main/SelectRace.png)


# Dependencies

The minimum Qt version to lunch these Application is 5.13.1. the file lastVersion_sauvegarde.sql have to be installed from Mysql . then the user have to link his 

database coordinates from dbconnection.cpp. 


# Installation

Install Qt Creator last version of Qt  Then install mysql from source.

```
sudo apt-get install libqt5sql5-mysql
```
```
sudo apt-get install libssl-dev
```
```
sudo apt-get install mysql-client
```
```
sudo apt-get install libmysqlclient-dev
```
```
sudo apt-get install libmysql++-dev
```
```
sudo apt-get install libmysqlcppconn-dev
```

Then user have to add DLL file of Mysql. this can be done on ubuntu like below: 

```

cd /usr/lib/x86_64-linux-gnu 
```
```
ldd libmysqlclient.so
```
```
cd ~/Qt/5.15.2/Src/qtbase/src/plugins/sqldrivers
```
```
~/Qt/5.15.2/gcc_64/bin/qmake sqldrivers.pro
```
```

make
```
```
make install 
```
```
cd /sqldrivers/mysql
```
```
~/Qt/5.15.2/gcc_64/bin/qmake mysql.pro
```
```
make
```
```
make install
```






