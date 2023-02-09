0x00. AirBnB clone - The console

https://github.com/Seamas007/AirBnB_clone/blob/master/README.md#author

This Project is done by the teams of 2 people ( Adefemi Oreyomi & Bosun Adebola)

https://github.com/Seamas007/AirBnB_clone/blob/master/README.md#project-description
This is the first part of the AirBnB clone project where we worked on the backend of the project whiles interfacing it with a console application with the help of the cmd module in python.

Data (python objects) generated are stored in a json file and can be accessed with the help of the json module in python

https://github.com/Seamas007/AirBnB_clone/blob/master/README.md#description-of-the-command-interpreter
The interface of the application is just like the Bash shell except that this has a limited number of accepted commands that were solely defined for the purposes of the usage of the AirBnB website.

This command line interpreter serves as the frontend of the web app where users can interact with the backend which was developed with python OOP programming.

Some of the commands available are:

show
create
update
destroy
count
And as part of the implementation of the command line interpreter coupled with the backend and file storage system, the folowing actions can be performed:

Creating new objects (ex: a new User or a new Place)
Retrieving an object from a file, a database etc…
Doing operations on objects (count, compute stats, etc…)
Updating attributes of an object
Destroying an object

https://github.com/Seamas007/AirBnB_clone/blob/master/README.md#how-to-start-it
These instructions will get you a copy of the project up and running on your local machine (Linux distro) for development and testing purposes.

https://github.com/Seamas007/AirBnB_clone/blob/master/README.md#installing

You will need to clone the repository of the project from Github. This will contain the simple shell program and all of its dependencies.

git clone https://github.com/jzamora5/AirBnB_clone.git
After cloning the repository you will have a folder called AirBnB_clone. In here there will be several files that allow the program to work.

/console.py : The main executable of the project, the command interpreter.

models/engine/file_storage.py: Class that serializes instances to a JSON file and deserializes JSON file to instances

models/__ init __.py: A unique FileStorage instance for the application

models/base_model.py: Class that defines all common attributes/methods for other classes.

models/user.py: User class that inherits from BaseModel

models/state.py: State class that inherits from BaseModel

models/city.py: City class that inherits from BaseModel

models/amenity.py: Amenity class that inherits from BaseModel

models/place.py: Place class that inherits from BaseModel

models/review.py: Review class that inherits from BaseModel


https://github.com/Seamas007/AirBnB_clone/blob/master/README.md#how-to-use-it

It can work in two different modes:

Interactive and Non-interactive.

In Interactive mode, the console will display a prompt (hbnb) indicating that the user can write and execute a command. After the command is run, the prompt will appear again a wait for a new command. This can go indefinitely as long as the user does not exit the program.

$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb) 
(hbnb) 
(hbnb) quit
$
In Non-interactive mode, the shell will need to be run with a command input piped into its execution so that the command is run as soon as the Shell starts. In this mode no prompt will appear, and no further input will be expected from the user.

$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 


