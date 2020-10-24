# Databases - Lab
## TEMP VERSION -- NOT FINAL
## Objective: 
In this lab, we will enhance the Confession bear website that we worked on in the previous lab.
We will move the storage of the previous lab from a dictionary to our database.

You will get to practice a bunch of your database skills, which is great!

#### Important keywords:
databases, sqlalchemy, schema, model, query


## Instructions:

1. Create 2 new files called `models.py`, and `database.py`.
   - `models.py` will contain our schemas.
   - `database.py` will contain our database actions. 
2. Create a new schema (model) for the subscribers, the model should contain: password, confession.
3. Create the following functions in `database.py`:
   - `add_confession(confession, password)` This function will create a new confession with the information given as parameters, it will create and return the confession_id for the specific confession.
   - `remove_confession(password)` This function will remove all the confessions from the database which matches the given password.
   - `get_confession(password)` This function returns the confession field if there is a confession matching the password given.
4. Make sure to test your code, use your functions to add rows to the database, and then use the other functions to interact with the rows you have added.
   - Move all information stored in the secrets dictionary to the database, each entry should be a row in the confessions table.

5. Now let's combine the newly created database with the website from Lab1.
   - In order to do this step, you must first complete the mandatory part of Lab1.
   - Copy `models.py` and `database.py` into your Lab1 project.
   - Import `database` in your `app.py` file.
   - Replace the use of a dictionary with the appropriate database functions.

##### Great job!
##### Call an Instructor/TA to check your completed tasks
 
 

## Bonus:

Implement any (or all) of the following features: (With no specific order)


#### Important keywords (for bonus):
Many to Many, One to Many, One to One, query
