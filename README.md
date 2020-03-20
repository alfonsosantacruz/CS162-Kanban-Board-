# CS162-Kanban-Board-
Kanban Board designed as part of my Web Application Assignment for my CS162-Software Engineering class during Spring 2020 in Hyderabad, India (Sophomore Year) at Minerva Schools at KGI.  Technologies used include Python, Flask, HTML, CSS and SQL.

# Simple Kanban-Board

Simple implementation of a Kanban Board with three sections "To do", "Doing", and "Done" created in Flask. 

<img width="943" alt="Rose's Kanban Board" src="https://user-images.githubusercontent.com/50888490/77203345-6b482c80-6aad-11ea-8964-ae8765ef9574.png">

## Features

1. Register new users. The password should contain at least 10 characters.
2. User authenitcation to Sign In.
3. Add tasks to any of the three categories in the board
4. Remove tasks at any stage.
5. Transfer tasks from "To Do" to "Doing", from Doing to Done and backwards from "Doing" to "To Do".
6. Logout from the web application, saving the unique credentials and tasks for access.
7. Access Slack, Google Calendar and Gmail in your web browser from the icons on the left for higher productivity.


Each user can have a Kanban board that is not accessible to other users.


##### Clone the repository to your local machine or get the master branch to run the web application.


## Windows

### Set Up Virtual Environment and Requirements

Open your CMD and type the following commands being in the Kanban directory
```python
python -m venv .venv
source .venv/Sources/activate
pip install -r requirements.txt
```

### Next, Set Up the Database

Being in the Kanban directory of your CMD, run the following from the Python shell (by typing python or python.exe in the cmd)
```python
from kanban import db
db.create_all()
exit()
```
 

### Run the App 

Being in the Kanban directory of your CMD:
```python
python kanban.py
```
Go to http://127.0.0.1:5000/ in your prefered Web-Browser


## To Run the Unit Tests 
 
It is suggested to open another cmd and while in the Kanban directory run the following:

```python 
python tests.py
```

Just make sure the app is running in http://127.0.0.1:5000/ while unit testing for an OK output.
If needed, change Flask debugger to active in line 187 of kanban.py



## macOS

### Set Up Virtual Environment and Requirements

Open your Terminal and type the following commands being in the Kanban directory
```python
python3.6 -m venv .venv
source .venv/bin/activate
pip3 install -r requirements.txt
```

### Next, Set Up the Database

Being in the Kanban directory of Terminal, run the following from the Python shell (by typing python3 in the cmd)
```python
from kanban import db
db.create_all()
exit()
```
 

### Run the App 

Being in the Kanban directory of your Terminal:
```python
python kanban.py
```
Go to http://127.0.0.1:5000/ in your prefered Web-Browser


## To Run the Unit Tests 
 
Being in the Kanban directory, access the "tests" directory in your Terminal, then run:

```python 
python tests.py
```

Just make sure the app is running in http://127.0.0.1:5000/ while unit testing for an OK output.
If needed, change Flask debugger to active in line 187 of kanban.py

References:

Build a User Login System With Flask-Login, Flask-WTForms, Flask-Bootstrap, and Flask-SQLAlchemy: https://www.youtube.com/watch?v=8aTnmsDMldY
Creating a Todo List App With Flask and Flask-SQLAlchemy: https://www.youtube.com/watch?v=4kD-GRF5VPs
