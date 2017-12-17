# Timeline
AS3 CPPS Emulator, written in Python.
Timeline is built heavily on Twisted and is even-driven, most of methods are Deferred too!

# Requirements
* Softwares:
  - Python >= 2.7
  - MySQL, with MySQL-c and MySQL-python connector
  - Redis server

* Python Modules: 
  - [Twisted](https://twistedmatrix.com)
  - [Watchdog](http://pythonhosted.org/watchdog/)
  - [txredisapi](https://github.com/fiorix/txredisapi)
  - [Twistar](http://findingscience.com/twistar/)
  - [BCrypt](https://pypi.python.org/pypi/bcrypt/)
  - [lxml](http://lxml.de/installation.html)
  - OPTIONAL : [colorlog](https://github.com/borntyping/python-colorlog)
  
# Installation and Usage
Download **Timeline**, put it in an accessable and readable directory. Navigate to that directory using CMD or Shell or any console client. Run `Start.py`. The server will start running.

You can edit `Start.py` to change `Handlers` module scope, `TCP` IP/Port endpoints, Logger etc. You can also add new methods!

Make sure you run **MySQL** and **Redis** server before starting the server.

You can query/run **database.sql** to build tables in your db.

# Default
* Default **database**          : **times-cp**
* Default **user**              : *username:* **test**, *password:* **password**
* Default **crumbs** directory  : **./configs/crumbs/**

**IMPORTANT :** By default Timeline uses colored logger, so you must install _'colorlog'_. If you wish not to use it and go by classical logger, change the following line
```py
TimelineLogger = InitiateColorLogger()
```
to
```py
TimelineLogger = InitiateLogger()
```

# Support
If you have any issue, found any bug or error or issue, or want to suggest some improvemnt, you are free to open an issue or request a pull request.
