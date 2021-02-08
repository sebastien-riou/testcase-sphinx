# testcase-sphinx

## Setup
This setup has been tested on Ubuntu 20.10 running as native OS and VirtualBox VM.

````
$ sudo apt-get install build-essential
$ sudo apt-get install zip
$ sudo apt install python3-pip
$ pip3 install pipenv
$ pipenv sync
````

if it does not work:
````
$ echo "export PATH=\$HOME/.local/bin:\$PATH" >> ~/.bashrc
$ sudo apt-get remove python3-pipenv
$ sudo pip3 install pipenv
$ sudo apt-get remove python3-virtualenv
$ sudo pip3 install virtualenv
````

open a new terminal or `source ~/.bashrc`

````
$ pipenv sync
````

To generate the html files:

````
$ cd docs
$ pipenv run make clean html
````

or

````
$ pipenv shell
$ cd docs
$ make clean html
````
