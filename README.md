EG-EMDR
=======

EMDR Consumer and batchs for EVE-Guidance project.

Important note
--------------

This "tool" is / will be a submodule for the main github project : https://github.com/Kyria/EVE-Guidance

Specific installation will be here, but if you want to use the whole application, please consider using the EVE-Guidance installation doc.

Project Requirements
--------------------
- Python >=2.7 <3 
- ZeroMQ
- MySQL (only for now)


Installation
------------

1. Create a virtual env ```
virtualenv egemdr_env
```
2. Go into the virtualenv and clone the repository ```
cd egemdr_env
git clone https://github.com/Kyria/EG-EMDR.git
``` 
3. Install requirements ``` 
source bin/activate
pip install -r EG-EMDR/requirements.txt
``` 
4. Configure the settings file in ```config```
5. On your database, execute ```sql/create_table.sql``` to create the required tables.
6. You are now ready to use it.

Using EG-EMDR
-------------

To use the emdr consumer, simply do this command : 
```
python consumer.py
```

You can call this python script in a daemon shell script to run it when you start your server. 
