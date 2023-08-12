## AirBnB clone - The console

## The AirBnB Clone
![AirBnB Logo](https://github.com/monoprosito/AirBnB_clone/raw/feature/console/hBnB.png?raw=true)

## Description
The project aims to build an Airbnb clone web application, and this first step involves implementing a command-line interface (CLI) that acts as a command interpreter. This is the initial phase of the AirBnB clone project, focusing on the backend development. We integrated it with a command-line application using Python's cmd module.
The CLI will allow us to perform various operations related to managing objects in the application, such as creating new objects (e.g., users, places), retrieving objects from storage, performing operations on objects (e.g., counting, computing stats), updating object attributes, and deleting objects.

To achieve this, the project will follow these steps:

**BaseModel Class**:
Implement a parent class called BaseModel that takes care of the initialization, serialization, and deserialization of instances. This class will act as the foundation for other classes in the project.

**Serialization/Deserialization Flow**:
Establish a flow to handle serialization/deserialization of objects. Instances will be converted to dictionaries, then to JSON strings, and finally, stored in files.

**Create Specific Classes**:
Create classes for the various entities in the Airbnb application, such as User, State, City, Place, etc. These classes will inherit from the BaseModel class.

**File Storage**:
Develop an abstracted storage engine for the project, specifically a file storage mechanism. This will handle reading and writing objects to files.

**Unit Tests**:
Write unit tests to validate the functionality of all the classes and the file storage engine. These tests will ensure that the application behaves correctly and reliably.

## Command Interpreter:
Build the actual command-line interface (CLI), which will act as the command interpreter. Users will interact with this interface to perform CRUD (Create, Read, Update, Delete) operations on the objects in the application.

By completing this first step, we'll have a solid foundation for your web application. we would be able to manage objects, serialize them, persist them to storage, and perform various operations on them. Subsequent steps in the project will build upon this foundation, integrating HTML/CSS templating, database storage, APIs, and front-end integration to create a fully functional Airbnb clone web application.

 The project is divided into different sub-projects which include:

AirBnB Clone - The Console
AirBnB Clone - Web static
AirBnB Clone - MySQL
AirBnB Clone - Deploy static
AirBnB Clone - Web framework
AirBnB Clone - RESTful API
AirBnB Clone - Web Dynamic

## The whole project is into 4 major parts and these are as follow:

The backend
The frontend
Storage
Testing

## The backend

This task involves applying object-oriented programming (OOP) concepts in Python. To successfully address this task, a solid understanding of various OOP principles is necessary. These principles encompass:

- **Classes:** Blueprint for creating objects. They define attributes and methods that objects will have.

- **Objects:** Instances of classes. They hold the actual data and can invoke the methods defined in the class.

- **Class and Instance Attributes:** Class attributes are shared among all instances of a class, while instance attributes are unique to each object.

- **Methods:** Functions defined within a class. They operate on the attributes of an object.

- **Inheritance:** The ability of a class to inherit attributes and methods from another class. It fosters code reuse and hierarchy.

In addition to these principles, proficiency in working with Python packages and modules is essential, particularly in importing modules and utilizing their functionalities.

For this project, there are two specific modules that are required:

1. **UUID Module:** This module assists in generating universally unique identifiers (UUIDs). UUIDs are unique identifiers used to distinguish objects even across different systems.

2. **Datetime Module:** This module facilitates working with date and time values. It enables tasks like obtaining the current date and time, formatting dates, and performing calculations involving time.

In essence, the project involves creating a Python package using OOP principles to model Airbnb objects. This necessitates knowledge of classes, objects, attributes, methods, and inheritance. Moreover, familiarity with the UUID and datetime modules is vital for generating unique IDs and managing date-time information.


In the project, the foundation involves creating a core model class that will serve as the base for all the other backend-oriented classes. This fundamental class will establish the essential structure and functionalities shared by the rest of the classes.

The project requires you to construct the following classes, each of which holds significance in the context of the Airbnb website:

- **User:** This class will manage user-related actions such as user registration and sign-up. Users are central to the Airbnb platform, and this class handles their interactions.

- **City:** The City class is responsible for dealing with city-related data. As Airbnb covers a wide range of locations, this class aids in managing information about different cities.

- **State:** Similar to the City class, the State class focuses on state-related data. It's essential for categorizing and organizing listings based on geographical regions.

- **Amenity:** The Amenity class pertains to amenities that can be associated with Airbnb places. Users will be able to list the amenities their places offer, and this class will facilitate that.

- **Place:** The Place class manages the listing of properties on the Airbnb platform. It handles details about the properties, their locations, and associated amenities.

- **Review:** This class deals with user reviews. Users can leave feedback for the places they've stayed, helping others make informed decisions.

These classes mirror the crucial functionalities of the Airbnb website that end users engage with. For instance, users can register, review places, and list their properties. The State class is instrumental in categorization, and amenities enhance property descriptions.

In summary, the project involves constructing a solid backend capable of handling a variety of actions and interactions, reflecting the core features of the Airbnb platform.

**The frontend**

The effectiveness of the project lies in providing the users with a way to interact with it, ensuring they don't need to directly access the underlying code. To achieve this, it's imperative to establish an interface that enables seamless communication between users and the backend.

In this specific project, the choice has been made to utilize the CMD (Command Line) module in Python. This decision stems from the fact that, at this stage, delving into learning HTML, CSS, and JavaScript – the technologies driving frontend development – hasn't been covered.

**Storage**

Another critical element in any web development endeavor involves managing data storage. While the ideal approach would be utilizing a database for this purpose, our project's context is such that we haven't yet delved into database technologies. Consequently, we were tasked with storing our data using a JSON file.

In order to successfully execute this task, it's necessary to gain a grasp of the JSON Module provided in Python. This module serves as a valuable tool for working with JSON data structures.

As a component of leveraging this module within the project, it's imperative to acquire an understanding of the processes of serialization and deserialization of Python objects. This entails converting data into a format suitable for storage (serialization) and then retrieving and reconstructing that data (deserialization). These skills are integral to effectively managing data storage within the context of our project's constraints.

By embracing the CMD module, you're crafting an avenue for users to engage with your application's functionalities via a command-line interface. This interface serves as a conduit that bridges the gap between users and the backend logic you've meticulously designed. Although more advanced frontend technologies like HTML, CSS, and JavaScript can offer immersive and interactive user experiences, the use of the CMD module aligns with the project's current scope, allowing you to effectively showcase your backend prowess.

Creating a Python Package:

A Python package is a way to organize related code into directories and modules. You create a package by organizing your code into a directory structure with __init__.py files in each subdirectory. This allows you to import and reuse your code across projects.

Creating a Command Interpreter with cmd Module:

The cmd module in Python allows you to create a simple command-line interface (CLI) with custom commands. You create a class that inherits from cmd.Cmd and define methods for each command.

Unit Testing and Implementing it in a Large Project:

Unit testing involves testing individual units (functions, methods, classes) of your code in isolation. It helps ensure that each component works as expected. For a large project, you can use testing frameworks like unittest, pytest, or nose. Write test cases that cover different scenarios and edge cases to validate your code's correctness.

Serializing and Deserializing a Class:

Serialization is the process of converting an object into a format that can be stored or transmitted, such as JSON or XML. Deserialization is the reverse process. Python provides libraries like json and pickle for serialization and deserialization.

Reading and Writing a JSON File:

The json module in Python allows you to work with JSON data. You can use json.dump() to write Python objects to a JSON file and json.load() to read data from a JSON file.

Managing Datetime:

The datetime module in Python provides classes and functions to work with dates and times. You can create datetime objects, perform arithmetic operations, and format them into strings.

UUID (Universally Unique Identifier):

A UUID is a 128-bit identifier that is unique across space and time. It's often used to uniquely identify objects or resources. Python's uuid module allows you to generate UUIDs.

args and How to Use It:

*args is used in function definitions to allow a variable number of non-keyword arguments. It collects extra positional arguments as a tuple.

kwargs and How to Use It:

**kwargs is used in function definitions to allow a variable number of keyword arguments. It collects extra keyword arguments as a dictionary.

Handling Named Arguments in a Function:

Named arguments (keyword arguments) in a function are provided using the key=value syntax. They allow you to pass arguments to a function in any order, making function calls more readable and flexible.
Data (python objects) generated are stored in a json file and can be accessed with the help of the json module in python

Description of the command interpreter:

The interface of the application is just like the Bash shell except that this has a limited number of accepted commands that were solely defined for the purposes of the usage of the AirBnB website.

This command line interpreter  serves as the frontend of the web app where users can interact with the backend which was developed with python OOP programming.

Some of the commands available are:
- show
- create
- update
- destroy
- count

And as part of the implementation of the command line interpreter coupled with the backend and file storage system, the folowing actions can be performed:
-   Creating new objects (ex: a new User or a new Place)
-   Retrieving an object from a file, a database etc…
-   Doing operations on objects (count, compute stats, etc…)
-   Updating attributes of an object
-   Destroying an object

## How to start it
These instructions will get you a copy of the project up and running on your local machine (Linux distro) for development and testing purposes.

## Installing

You will need to clone the repository of the project from Github. This will contain the simple shell program and all of its dependencies.

After cloning the repository you will have a folder called AirBnB_clone. In here there will be several files that allow the program to work.

> /console.py : The main executable of the project, the command interpreter.
>
> models/engine/file_storage.py: Class that serializes instances to a JSON file and deserializes JSON file to instances
>
> models/__ init __.py:  A unique `FileStorage` instance for the application
>
> models/base_model.py: Class that defines all common attributes/methods for other classes.
>
> models/user.py: User class that inherits from BaseModel
>
>models/state.py: State class that inherits from BaseModel
>
>models/city.py: City class that inherits from BaseModel
>
>models/amenity.py: Amenity class that inherits from BaseModel
>
>models/place.py: Place class that inherits from BaseModel
>
>models/review.py: Review class that inherits from BaseModel



## How to use it
It can work in two different modes:


**Interactive** and **Non-interactive**.

In **Interactive mode**, the console will display a prompt (hbnb) indicating that the user can write and execute a command. After the command is run, the prompt will appear again a wait for a new command. This can go indefinitely as long as the user does not exit the program.

```
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb)
(hbnb)
(hbnb) quit
$
```

In **Non-interactive mode**, the shell will need to be run with a command input piped into its execution so that the command is run as soon as the Shell starts. In this mode no prompt will appear, and no further input will be expected from the user.


```
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
$
```

## Format of Command Input

In order to give commands to the console, these will need to be piped through an echo in case of  **Non-interactive mode**.

In  **Interactive Mode**  the commands will need to be written with a keyboard when the prompt appears and will be recognized when an enter key is pressed (new line). As soon as this happens, the console will attempt to execute the command through several means or will show an error message if the command didn't run successfully. In this mode, the console can be exited using the **CTRL + D** combination,  **CTRL + C**, or the command **quit** or **EOF**.

## Arguments

Most commands have several options or arguments that can be used when executing the program. In order for the Shell to recognize those parameters, the user must separate everything with spaces.

Example:

```

ubuntu:~/AirBnB$ ./console.py
(hbnb) create BaseModel
49faff9a-6318-451f-87b6-910505c55907
ubuntu:~/AirBnB$ ./console.py

```

or

```
ubuntu:~/AirBnB$ ./console.py $ echo "create BaseModel" | ./console.py
(hbnb)
e37ebcd3-f8e1-4c1f-8095-7a019070b1fa
(hbnb)
ubuntu:~/AirBnB$ ./console.py
```

## Available commands and what they do

The recognizable commands by the interpreter are the following:

|Command| Description |
|--|--|
| **quit or EOF** | Exits the program |
| **Usage** | By itself |
| **-----** | **-----** |
| **help** | Provides a text describing how to use a command.  |
| **Usage** | By itself --or-- **help <command\>** |
| **-----** | **-----** |
| **create** | Creates a new instance of a valid `Class`, saves it (to the JSON file) and prints the `id`.  Valid classes are: BaseModel, User, State, City, Amenity, Place, Review. |
| **Usage** | **create <class name\>**|
| **-----** | **-----** |
| **show** | Prints the string representation of an instance based on the class name and `id`  |
| **Usage** | **show <class name\> <id\>** --or-- **<class name\>.show(<id\>)**|
| **-----** | **-----** |
| **destroy** | Deletes an instance based on the class name and `id` (saves the change into a JSON file).  |
| **Usage** | **destroy <class name\> <id\>** --or-- **<class name>.destroy(<id>)** |
| **-----** | **-----** |
| **all** | Prints all string representation of all instances based or not on the class name.  |
| **Usage** | By itself or **all <class name\>** --or-- **<class name\>.all()** |
| **-----** | **-----** |
| **update** | Updates an instance based on the class name and `id` by adding or updating attribute (saves the changes into a JSON file).  |
| **Usage** | **update <class name\> <id\> <attribute name\> "<attribute value\>"** ---or--- **<class name\>.update(<id\>, <attribute name\>, <attribute value\>)** --or-- **<class name\>.update(<id\>, <dictionary representation\>)**|
| **-----** | **-----** |
| **count** | Retrieve the number of instances of a class.  |
| **Usage** | **<class name\>.count()** |


The variable `dtime_format` in the context of your project is a string that represents a specific format for date and time strings. It uses special format codes to define how date and time components are represented.

In this case, the format is `'YYYY-MM-DDTHH:MM:SS.ssssss'`, where each part has a specific meaning:

- `'YYYY'`: Represents the year with four digits (e.g., 2023).
- `'MM'`: Represents the month with two digits (e.g., 08 for August).
- `'DD'`: Represents the day of the month with two digits (e.g., 04).
- `'T'`: A literal character 'T' used as a separator.
- `'HH'`: Represents the hour with two digits (e.g., 12 for 12 PM).
- `'MM'`: Represents the minute with two digits (e.g., 34).
- `'SS'`: Represents the second with two digits (e.g., 56).
- `'.ssssss'`: Represents the microsecond with six digits (e.g., 789012).

An example of a date and time string formatted using this `dtime_format` would look like this:

```
2023-08-04T12:34:56.789012
```

When you have a date and time string in this specific format, you can use Python's `datetime.strptime()` method to convert it into a `datetime` object:

```python
from datetime import datetime

date_time_str = '2023-08-04T12:34:56.789012'
dtime_obj = datetime.strptime(date_time_str, dtime_format)
print(dtime_obj)
```

This will output:
```
2023-08-04 12:34:56.789012
```

Similarly, you can use the `strftime()` method of a `datetime` object to format it back to the desired string format:

```python
formatted_str = dtime_obj.strftime(dtime_format)
print(formatted_str)
```

This will output:
```
2023-08-04T12:34:56.789012
```

The `dtime_format` variable provides a standard representation of date and time strings, making it easier to parse and format date and time data consistently within your project.


In the context of the Airbnb clone project, the `BaseModel` class serves as the parent or base class for other classes representing various entities in the application. It provides common functionality that can be inherited and used by its child classes. Here's an example implementation of the `BaseModel` class:

```python
import uuid
import json

class BaseModel:
    def __init__(self, *args, **kwargs):
        # Assign a unique identifier to each instance
        self.id = str(uuid.uuid4())
        # Set the creation time for the instance
        self.created_at = datetime.now()
        # Update the instance attributes using kwargs
        for key, value in kwargs.items():
            setattr(self, key, value)

    def to_dict(self):
        """Converts the instance attributes to a dictionary."""
        # Get a dictionary representation of the instance
        obj_dict = self.__dict__.copy()
        # Remove the '__class__' key as it's not needed for serialization
        obj_dict.pop('__class__', None)
        # Convert the 'created_at' attribute to an ISO formatted string
        obj_dict['created_at'] = self.created_at.isoformat()
        return obj_dict

    def __str__(self):
        """Returns a string representation of the instance."""
        class_name = self.__class__.__name__
        return "[{}] ({}) {}".format(class_name, self.id, self.__dict__)

    def save(self):
        """Saves the instance data to a file in JSON format."""
        filename = "{}.json".format(self.id)
        with open(filename, 'w') as file:
            json.dump(self.to_dict(), file)

    @classmethod
    def load(cls, filename):
        """Loads an instance from a JSON file and returns the instance."""
        with open(filename, 'r') as file:
            data = json.load(file)
        # Return a new instance with the loaded data
        return cls(**data)
```

Explanation of the `BaseModel` class:

1. The `__init__` method is the constructor of the class. It sets the `id` and `created_at` attributes for each instance and allows additional attributes to be initialized through keyword arguments (`kwargs`).

2. The `to_dict` method converts the instance attributes into a dictionary, preparing it for serialization to JSON.

3. The `__str__` method provides a human-readable string representation of the instance.

4. The `save` method serializes the instance data to a JSON file with the name `{id}.json`.

5. The `load` method is a class method that allows you to load an instance from a JSON file.

Child classes like `User`, `State`, `City`, `Place`, etc., will inherit from the `BaseModel` class and can use its methods and attributes. These child classes will define their own specific attributes and methods, customizing the behavior for their respective entities in the Airbnb application.

## To create a Python package structure for the project:

 airbnb/
  |-- __init__.py
  |-- models/
  |     |-- __init__.py
  |     |-- base_model.py
  |     |-- user.py
  |     |-- state.py
  |     |-- city.py
  |     |-- place.py
  |-- storage/
  |     |-- __init__.py
  |     |-- engine.py
  |     |-- file_storage.py
  |-- tests/
  |     |-- __init__.py
  |     |-- test_base_model.py
  |     |-- test_user.py
  |     |-- test_state.py
  |     |-- test_city.py
  |     |-- test_place.py
  |     |-- test_file_storage.py
  |-- console.py

  Here's a brief overview of each component:

models/: This package contains the classes representing Airbnb objects (e.g., User, State, etc.).

storage/: This package contains the storage engine implementations (e.g., FileStorage).

tests/: This package contains unit tests for the classes and storage engine.

console.py: This is the command interpreter (CLI) using the cmd module. It's responsible for handling user input and interacting with the classes and storage engine.


## Author

**Esther Ejimofor** && **Emmanuel Nmaju**
