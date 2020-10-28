# Databases - Lab

## Objective: 
In this lab, we will enhance the Confession bear website that we worked on in the previous lab.
We will move the storage of the previous lab from a dictionary to our database.

You will get to practice a bunch of your database skills, which is great!

#### Important keywords:
databases, sqlalchemy, schema, model, query


## Instructions:
> Remember, you can view all of our lectures, labs, and pre-recorded lectures [here](https://tinyurl.com/y2yl-material)


1. Create 2 new files in your main project foler, called `model.py`, and `database.py`.
   - `model.py` will contain our schemas and database tables.
   - `database.py` will contain our database actions. 
2. Create a new database table (in `model.py`) for the **subscribers**, the table should contain: password, confession.
   - hint: don't forget about the `id`!
3. Create the following functions in `database.py`:
   - `add_confession(confession, password)` This function will create a new confession with the information given as parameters, it will create and return the `confession_id` for the specific confession.
   - `remove_confession(password)` This function will remove all the confessions from the database which matches the given password.
   - `get_confession(password)` This function returns the confession field if there is a confession matching the password given.
   - *Hint: Don't forget to import model in `database.py`.*
4. Make sure to test your code, use your functions to add rows to the database, and then use the other functions to interact with the rows you have added.
   - Move all information stored in the secrets dictionary to the database, each entry should be a row in the confessions table.

5. Now let's combine the newly created database with the website from `Lab1`.
   - In order to do this step, you must first complete the mandatory part of Lab1.
   - Make sure `model.py` and `database.py` into your Lab1 project folder.
   - Import `database` in your `app.py` file.
   - Replace the use of a dictionary with the appropriate database functions.

##### Great job!
##### Call an Instructor/TA to check your completed tasks
 
 

## Bonus:

Implement any (or all) of the following features: (With no specific order)

* For any (or all) bonuses that exist in Lab1:
  - Update your database schemas, create database functions, and update your website's code such that all information is saved on the database.
  - You should start by updating for the bonuses you have already implemented. If you want, you may implement more of the Lab1 bonuses.
* Create a `"/admin"` page:
  - This page will require a password.
  - After inserting password, the admin user can:
    - See a list of all secrets sorted by their task, without seeing their passwords.
    - Delete any secret that's on the website.
* Add a view count for each secret. (Should appear on the page and be stored in the database as well.)
* Add a report button for secrets. The report button would be used to flag inappropriate content.
  - After pressing the report button, a text screen will appear, allowing the user to voice his concerns.
  - The report will be saved in the database. (You should plan out how.)
  - If you have implemented an admin user (from the bonuses): Add a page called `"/reports"`:
    - The page should allow an admin user to view all reports, and the text for confessions relating to them.
    - The page will also include buttons to decline a report, removing it, and to accept a report, removing the related confession and the report.

_Note_: All those features require multiple steps in order to implement, start out by planning those steps, and then implement them, make sure to test your code often.

#### Important keywords (for bonus):
One to Many relationship, Cookies
