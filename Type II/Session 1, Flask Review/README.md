# Javascript I - Lab

## Objective: 
In this lab, you will create a secrets' website called: Confession Bear!
The website will contain secrets, each one of them will be protected by a different password!

In general terms, your website would look like this:

<img src="https://i.ibb.co/WKmzXCY/website-diagram.png" alt="website-diagram" border="0" width="500">

Currently we are going to set the secrets statically, which means we will define the secrets, and users are not able to add new secrets.


## Instructions:

1. Create a new flask project.

2. Create a page for password input.
  a. Link the page to the homepage url. ("/")
  b. Create a new template for the page, the template should contain a form which allows you to enter a password and a submit page.
  c. Write the code that shows the page.
  d. Run your code to make sure that it's working in this stage! :)
  
3. Create a bunch of secrets.
  a. In your code, create a CONST variable, containing a dictionary, the keys for dictionary are passwords for the secrets, the values are the contents of each secret. (Have at least 2 secrets)
  b. Create a template for the secret presentation page. (Make sure you can dynamically insert the secret's contents.)
  c. Link the template to the following url: "/password_input".
  d. Run your code to make sure that it's working in this stage! :)

4. Edit the page to process the form.
 a. Allow the POST method for the "/password_input" page.
 b. Edit the teamplate of the homepage, such that the form sends a POST request to "/password_input"
 c. Edit the "/password_input" function, such that it compares to see whether the password received from the request matches one of the passwords that we have. If the password matches, you should show the appropriate secret, otherwise, you should show the homepage instead.
 d. Run your code to make sure that it's 
 



##### Great job!
##### Call an Instructor/TA to check your completed tasks
 
 


## Bonus:

<img src="https://www.c-sharpcorner.com/UploadFile/201fc1/programming-in-java-using-the-mvc-architecture/Images/mvc%20framework.jpg" width="350">
