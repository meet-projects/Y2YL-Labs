# Javascript I - Lab

## Objective: 
In this lab, you will:
- Continue working on the labs from the previous session.
- Build a page to display the picture from the Mars rover.





<img src="https://www.popsci.com/resizer/sLoHrJJ8stQeU6XEhU6jmfkdzjM=/760x506/arc-anglerfish-arc2-prod-bonnier.s3.amazonaws.com/public/WCWFYS3C6MNHW6RTXZJ5F6EU2M.gif" width="400">





## Instructions:
> API: https://api.nasa.gov/mars-photos/api/v1/rovers/curiosity/photos?sol=1000&api_key=DEMO_KEY



### Part 1 - Setup:
- Go to app.py and import all the necessary libraries (json, requests, etc.)
- Define and create a route for the function display().

### Part 2 - using the API:
- The display() function should:
 - Retrieve the information from the API (use the requests.get() function) and parse its content (parsing a JSON string means turning it into a python dictionary).
 - Return the link of the first picture. (http://mars.jpl.nasa.gov/msl-raw-images/proj/msl/redops/ods/surface/sol/01000/opgs/edr/fcam/FLB_486265257EDR_F0481570FHAZ00323M_.JPG) 

### Part 3 - Building the website:
- Create an HTML template show_pic.html that will display the picture (use flask variables, how?).
- The display() function should render the template, and pass the picture’s link to the template.





##### Great job!
##### Call an Instructor/TA to check your completed tasks
 
 


## Bonus:
- Create another route (use a variable route, receives an integer variable called picture_id) which executes the function picture(picture_id) (which you’ll need to define).
 - The function picture(picture_id) will:
  - Render the template show_picture.html.
  - Pass the link of the picture to the template so the picture would be displayed.
- To the template show_template.html, add navigation buttons (left and right) to move to the next/previous picture.
