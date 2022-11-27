0x00. AirBnB clone - The console
_________________________________________________

The Overview
_______________________________________________

Airbnb is a popular website that is dirupting the hospitality industry by giving people the power to rent out rooms in their homes and rent wherever they choose. With Airbnb, hosts can list their spaces and book unique accomodations.
Our assignment is to clone Airbnb and for this assignment our goal is to creat the console with python. The console is important for the overall success of the project because it allows to create, destroy, show, save, and update our BaseModel,, a framework that is inheritable by other classes or catgoires.

___________________________________________________________________________________ How to start console
AirBnB_clone$ ./console.py
(hbnb) 
(hbnb) 
(hbnb) all
[]
 How to use console
  - to create a new user
   
(hbnb) User.create()
1bab8a19-a0c7-43ef-956b-b3271bdd684f
(hbnb) User.all()
["[User] (1bab8a19-a0c7-43ef-956b-b3271bdd684f) {'updated_at': datetime.datetime(2017, 10, 4, 18, 21, 27, 164392), 'email': '', 'created_at': datetime.datetime(2017, 10, 4, 18, 21, 27, 164366), 'last_name': '', 'password': '', 'id': '1bab8a19-a0c7-43ef-956b-b3271bdd684f', 'first_name': ''}"]_
 This is a best example to create a user

  - to show a specific user you will "show" command and takes in two agreements the name and the ID

(hbnb) show User 777f8007-5aeb-4568-8334-807d507edce0
[User] (777f8007-5aeb-4568-8334-807d507edce0) {'updated_at': datetime.datetime(2017, 10, 4, 18, 21, 59, 114711), 'email': '', 'created_at': datetime.datetime(2017, 10, 4, 18, 21, 59, 114685), 'last_name': '', 'password': '', 'id': '777f8007-5aeb-4568-8334-807d507edce0', 'first_name': ''}


__________________________________________________________________________
To destroy a User, use the "destroy" command. The command takes in two arguments - name and id. When successfully implemented, destroy will delete the User from file storage. Please see example below:

(hbnb) create User
06505348-0c86-4273-b1c2-68eefcbbab0c
(hbnb) show User 06505348-0c86-4273-b1c2-68eefcbbab0c
[User] (06505348-0c86-4273-b1c2-68eefcbbab0c) {'id': '06505348-0c86-4273-b1c2-68eefcbbab0c', 'last_name': '', 'updated_at': datetime.datetime(2017, 10, 4, 19, 18, 40, 976205), 'email': '', 'created_at': datetime.datetime(2017, 10, 4, 19, 18, 40, 976174), 'password': '', 'first_name': ''}
(hbnb) destroy User 06505348-0c86-4273-b1c2-68eefcbbab0c
(hbnb) show User 06505348-0c86-4273-b1c2-68eefcbbab0c
** no instance found **
__________________________________________________________________________
The "all" command prints all string representation of all instances and the "update" command is used to update the User information, 

(hbnb) update BaseModel 49faff9a-6318-451f-87b6-910505c55907 first_name "Betty"
(hbnb) show BaseModel 49faff9a-6318-451f-87b6-910505c55907
[BaseModel] (49faff9a-6318-451f-87b6-910505c55907) {'first_name': 'Betty', 'id': '49faff9a-6318-451f-87b6-910505c55907', 'created_at': datetime.datetime(2017, 10, 2, 3, 10, 25, 903293), 'updated_at': datetime.datetime(2017, 10, 2, 3, 11, 3, 49401)}
__________________________________________________________________________________

Requirements
Python Scripts
Allowed editors: vi, vim, emacs
All your files will be interpreted/compiled on Ubuntu 20.04 LTS using python3 (version 3.8.5)
All your files should end with a new line
The first line of all your files should be exactly #!/usr/bin/python3
A README.md file, at the root of the folder of the project, is mandatory
Your code should use the pycodestyle (version 2.8.*)
All your files must be executable
The length of your files will be tested using wc
All your modules should have a documentation (python3 -c 'print(__import__("my_module").__doc__)')
All your classes should have a documentation (python3 -c 'print(__import__("my_module").MyClass.__doc__)')
All your functions (inside and outside a class) should have a documentation (python3 -c 'print(__import__("my_module").my_function.__doc__)' and python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)')
A documentation is not a simple word, it’s a real sentence explaining what’s the purpose of the module, class or method (the length of it will be verified)
___________________________________________________________________________

Python Unit Tests
Allowed editors: vi, vim, emacs
All your files should end with a new line
All your test files should be inside a folder tests
You have to use the unittest module
All your test files should be python files (extension: .py)
All your test files and folders should start by test_
Your file organization in the tests folder should be the same as your project
e.g., For models/base_model.py, unit tests must be in: tests/test_models/test_base_model.py
e.g., For models/user.py, unit tests must be in: tests/test_models/test_user.py
All your tests should be executed by using this command: python3 -m unittest discover tests
You can also test file by file by using this command: python3 -m unittest tests/test_models/test_base_model.py
All your modules should have a documentation (python3 -c 'print(__import__("my_module").__doc__)')
All your classes should have a documentation (python3 -c 'print(__import__("my_module").MyClass.__doc__)')
All your functions (inside and outside a class) should have a documentation (python3 -c 'print(__import__("my_module").my_function.__doc__)' and python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)')
We strongly encourage you to work together on test cases, so that you don’t miss any edge case
