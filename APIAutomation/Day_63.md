## Learning Goal
Http Status codes

### Resources
- https://developer.mozilla.org/en-US/docs/Web/HTTP/Status
- https://docs.telerik.com/fiddler/knowledge-base/autoresponder#creating-autoresponder-rules

### Problem statement
Open the URL https://home.openweathermap.org/users/sign_in and intercept the various requests using fiddler. 
Simulate different status codes from fiddler and validate the error messages from browser.

### Steps to follow
- Open fiddler tool and start capturing traffic
- Open the url mentioned above and click on submit button
- Once the request is captured, select the response and go to the autoreponder tab
- Click on Add rule
- Select the response to be returned from the dropdown Local file to return
- Select any status code from the dropdown for example 502_Unreachable.dat and save the changes.
- Click on enable rules checkbox.
- Go to the browser and refresh the page.
- Validate you have seen the response as sent from fiddler.
- Close fiddler and verify that web page is returning response as before.
- Explore the different error codes in similar way.

Notes: Fiddler Autoresponder can be used for this challenges.
