# NotchUp Interview Assignment
This is a web app to book trial class on NotchUp education platform

[![screenshot](./original_assets/screenshot.png)](https://www.youtube.com/watch?v=jDvAg_5acSI)        
[![demo video](./original_assets/thumbnail.png)](https://www.youtube.com/watch?v=jDvAg_5acSI)      

* [Web app](https://notchup-test.web.app/)        
* [Frontend code](https://github.com/atiqg/NotchUp-test/tree/main/public)      
* [Backend code](https://github.com/atiqg/NotchUp-test/tree/main/functions)     
<br>

## Assignment:       
### Part 1A:       
[✔️] - Build a webpage with a form that people can use to book a trial class on notchup.co. The form should be able to capture user and class details      
[✔️] - Fetch courses from NotchUp       
[✔️] - Each trial slot is for 1 hour duration        
[✔️] - Slots are fetched from a GET request (Details below) and each timeslot is in unixtime format.       
[✔️] - Earliest slot we can show should be minimum 4 hours from now.        
[✔️] - Latest slot should be maximum 7 days from now.       
[✔️] - On submitting the form, you may simply clear the form without needing to post that data.       

### Part 1B:        
[✔️] - The data submitted through the form needs to be sent to a server which is responsible for sending out confirmation email to the users.      
[✔️] - Set up an API on a node JS server that can take the form submission fields as an input.       
[✔️] - On each submission, the server should send out an email on the given parent's email id.         
[✔️] - Host the webpage on a free hosting service like sites.google.com or herokuapp.com. Reply to this email with a link of the webpage.     
[✔️] CSS    


## installation & usage      
```
git clone https://github.com/atiqg/NotchUp-test.git
cd NotchUp-test/functions
npm install
firebase functions:config:set gmail.email="<user@gmail.com>" gmail.password="<GMAIL_APP_PASSWORD>"
cd ..
firebase deploy
```

use resulting url to access web app 


## troubleshoot
* This project is using NotchUp api endpoint to fetch courses and their available time slots, so things can go wrong in future. If so, use [saved time slots file](./original_assets/saved_time_slots.json)             
* Time slots are old so I am bumping them X days ahead [here](https://github.com/atiqg/NotchUp-test/blob/99cd38b88ef881555b2a8e234758a680c45af8c7/public/script.js#L71)       
* Importing firebase project can cause problems so direclty use functions/index.js file in fresh fireabse function project
