# Software needed for BI class

## Python

We will need Python > 3.5 version.
Linux and Mac users should have both 2.7.x and > 3.6.x versions installed by default on their machines. You can check your current version for both of them with:

```
python --version
python3 --version
```

![alt text](https://github.com/karolosk/bi_software/blob/gh-pages/pythonv.png)

Windows users please go at https://www.python.org/downloads/windows/ and get the appropriate file for your PC. Please note that during the installation you will be asked to add Python in Path. You should enable this option. 

![alt text](https://github.com/karolosk/bi_software/blob/gh-pages/pythonpath.png)

It allows you to run your files on cmd by: 

```
python python_file.py
```

If you do not enable this you will be forced to use the full python path to execute your programs. (for example, it will be something like: 
c:/users/username/program files/python36/python pytthon_file.py )

## IDE 

This is up to you. Some recommendations:
- VS Code https://code.visualstudio.com/download)
- PyCharm Community edition (https://www.jetbrains.com/pycharm/downloadr

## PostgreSQL 

Labs will be PostgreSQL based from the relational aspect. Documentation for PostgreSQL can be found here https://www.postgresql.org/docs/ depending on the version you will use (> 9.5). 
If you want to have your database on your machine you can download it from here: 
https://www.postgresql.org/download/ and choose depending on your OS.


Also you should have ready any IDE that you prefer in order to have a GUI to your database. PostgreSQL also offers the relevant tool PGAdmin (version 4). 

Below you can find some installation notes for Windows and Ubuntu 18.04 for PostgreSQL 10.


### Windows 

There is a typical installer for Windows. The installation is normal and at some point you will have to choose components. You may choose the components you want to install in your system. You may uncheck Stack Builder but keep the rest. 
Later you will have to enter a superuser password. Make a note of it. This is to access the whole instance not a specific database. At the last screen of the installer uncheck the Stack Builder option. 

Then you will be ready to access your local Postgres via PGAdmin. 

Find PgAdmin from search and launch it. This will lead to PGAdmin homepage

Click on Servers -> PostgreSQL 10 and you will be prompted to enter the password you set during installation. You should be able to see the dashboard now.

### Ubuntu

There are several ways to install in Ubuntu and that depends on the OS version as well. 
Below example is for 18.04. 

In 18.04’s repositories PostgreSQL 10 is included. 
Type in your terminal:
sudo apt update
sudo apt install postgresql postgresql-contrib

You will be prompted to enter a password for the superuser as we mentioned earlier in Windows notes


And then to get PGAdmin if you want it:
sudo apt install pgadmin4
