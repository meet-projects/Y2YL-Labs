# Flask Forms - Lab

## Objective: 
In this lab, you will ...





<img src="https://www.nasa.gov/sites/default/files/thumbnails/image/xemu-eva-hls.jpg" width="400">





## Instructions:
1. Open your repl.it from the previous lab.
2. Edit the login route, to allow `GET` and `POST` methods.
3. Edit the form tag in `login.html` in order to link it correctly to our login route. 
    - Set the `action` to the login route `'/'`, and the `method` to `"POST"`.
4. Inside the login fuction:
    i. Don't forget, to check the method (Get/Post) in order to continue to the next steps.
    ii. Assign allowed usernames and passwords, which means; create variables defining the correct username and password that should be allowed if entered.
        - For example:  
        ```python
        username = "Jiana"
        password = "meetyear2022"
        
        @app.route(.........
        ```
    iii. Check if the information is correct. 
        - If it is → proceed to logging in the portal (home page). 
        - If not → try logging in again.
5. When returning the `"Portal.html"`, pass the `username`, so it will display `“Welcome, [username]”` when logged in.





##### Great job!
##### Call an Instructor/TA to check your completed tasks
 
 


## Bonus:

<img src="https://www.c-sharpcorner.com/UploadFile/201fc1/programming-in-java-using-the-mvc-architecture/Images/mvc%20framework.jpg" width="350">
