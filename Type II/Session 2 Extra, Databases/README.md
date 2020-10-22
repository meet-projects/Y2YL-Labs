# Databases - Lab

## Objective: 
In this lab, you will create a database for the amazing subscribers of the imaginary organization: Humans for a non-specific cause.
You will get to practice a bunch of your database skills, which is great!

#### Important keywords:
databases, sqlalchemy, schema, model, query


## Instructions:

1. Create 2 new files called `models.py`, and `database.py`.
   - `models.py` will contain our chemas.
   - `database.py` will contain our database actions. 
2. Create a new schema (model) for the subsribers, the model should contain: username, password. (username must be unique.)
3. Create the following functions in `database.py`:
   - `add_subscriber(username, password)` This function will create a new subscriber with the information given as parameters.
   - `remove_subscriber(username)` This function will remove the subscriber from the database which has the given username.
   - `get_all_subscribers()` This function will return a list of all the subscribers' usernames.
   - `validate_subscriber(username, attempt_password)` This function returns True if there is a user matching the username and the password given is that user's password, returns False otherwise.
4. Make sure to test your code, user your functions to add rows to the database, and then use the other functions to interact with the rows you have added.

##### Great job!
##### Call an Instructor/TA to check your completed tasks
 
 

## Bonus:

Implement any (or all) of the following features: (With no specific order)

* Add `join_time` to the subscriber schema, this column represents the join time of a user.
  - The join time is added and calculated automatically by `add_subscriber`
  - `get_all_subscribers` now returns the list ordered by the join time, newest first.
* Add a new schema for branches of the organization. Branches have an id, a name, an address, and a motto.
  - Each subscriber belongs to address, change the subscriber schema to add the branch for each subscriber. (Each subsriber belongs to one branch exactly)
  - Add the following functions to `database.py`:
    - `get_subscriber_branch(username)` This function will get all branch information for the given username.
    - `get_all_branch_subscribers(branch_id)` This function will get the names of all subscribers who belong to the branch with the given id. (Empty list if there are no subscribers)
* Add relationship status between subscribers, any 2 subscribers can have any of the following relationship: romance, rivalry, friendship, family, resentment. They can also have no relationship at all.
  - Add the following functions to `database.py`:
    - `get_all_relationship(status)` This function will get pairs of names of subscribers that have the matching relationships.
    - `get_relationship_of(username1, username2)` Get the relationship of the two subscribers denoted by the username if it exists, return `None` otherwise.
* Add a mentor figure for the subscriber, the mentor is another subscriber. Every subscriber must have exactly one mentor. (A subscriber can be his own mentor.)
  - Add the following functions to `database.py`:
    - `get_mentor(username)` Get the name of the mentor of the given user.
    - `get_mentees(username)` Get a list of all subscribers who have the given username as their mentor.

#### Important keywords (for bonus):
Many to Many, One to Many, One to One, query
