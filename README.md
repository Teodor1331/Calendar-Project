# Calendar

Calendar Application made on Python Language and the Flask framework

The calendar application is a peculiar substite of the groups in Facebook and
is like a combination of these groups and Google Calendar. This application is
developed on Ubuntu 18.04.

Little steps of how to run your application.

First your must have Python 3 and PIP installed from Python 3 version of the language.
To check if you have already installed them on your machine, type these commands one by one:

```
python3 --version
pip3 --version

```

If you have them, pass the next commands, but if you haven't them, install them with
these commands, again one by one. Important: after every new command you may need to
type your password for using your operational system.

```
sudo apt install python3.9
sudo apt install python3-pip
```

It is good to upgrade your Python and PIP version to the newest with:

```
sudo apt update
python3 -m pip install --upgrade pip
```


The next thing you should do is to install the virtual environment. For that purpose
you will need to type this command:

```
pip3 install virtualenv
```

For the installation of the project, navigate to the project folder and pass the first 
command from below if your are already in it. The name of the folder is "Calendar", but
after downloading the folder you will see the name "Calendar-master". Then you must
type the next commands:

```
cd Calendar-master/
sudo apt-get install libffi-dev
virtualenv env
source env/bin/activate
pip3 install -r requirements.txt
```

After this enter these commands for creating the base of data. You have to go in the
Python console mode, type the needed commands and then exit from the Python console:

```
python3
from main import db
db.create_all()
exit()
```

The last commands you should type are:

```
export FLASK_APP=main.py
export FLASK_DEBUG=1
export FLASK_ENV=development
flask run
```
