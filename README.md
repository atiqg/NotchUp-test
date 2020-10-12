# NotchUp Interview Assignment
This is web app to book trial class on NotchUp education platform

* [Web app](https://notchup-test.web.app/)        
* [Frontend code](https://github.com/atiqg/NotchUp-test/tree/main/public)      
* [Backend code](https://github.com/atiqg/NotchUp-test/tree/main/functions)     
<br>

## Assignment:       
### Part 1A:       
[x] - Build a webpage with a form that people can use to book a trial class on notchup.co. The form should be able to capture user and class details      
[x] - Fetch courses from NotchUp       
[x] - Each trial slot is for 1 hour duration        
[x] - Slots are fetched from a GET request (Details below) and each timeslot is in unixtime format.       
[x] - Earliest slot we can show should be minimum 4 hours from now.        
[x] - Latest slot should be maximum 7 days from now.       
[x] - On submitting the form, you may simply clear the form without needing to post that data.       

### Part 1B:        
[x] - The data submitted through the form needs to be sent to a server which is responsible for sending out confirmation email to the users.      
[x] - Set up an API on a node JS server that can take the form submission fields as an input.       
[x] - On each submission, the server should send out an email on the given parent's email id.         
[x] - Host the webpage on a free hosting service like sites.google.com or herokuapp.com. Reply to this email with a link of the webpage.     
[ ] CSS    