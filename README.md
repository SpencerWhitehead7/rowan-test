# Not-Yelp

## Build and Run Directions

Go to https://sw7-not-yelp.herokuapp.com/ and use app

OR:

Clone repo

Get secrets.js file from me and add it to root of project directory

Run ```npm install``` in command line from project folder

Run ```npm run start``` in command line from project folder

(use ```npm run start-dev``` instead if you want to be able to change files and see the results (after a reload) on the localhost site)

Go to http://localhost:1337 in browser

Of course, you can clone the repo, look at the code, and run on a localhost without the secrets.js file, you just can't (successfully) call the Yelp API.

## Technologies

I used:

Express to proxy my query to the Yelp API instead of querying directly from the front end with Axios so I could store the API access token securely. Express also makes serving a React site fairly convenient.

React for the front end because it allows you to create reusable components, track your app's internal state (which is helpful for a project that's loading things, juggling different sets of data and variables, and occasionally erroring out), and render components conditionally. The app was not complex enough to warrant using something like Redux to provide a common state to multiple components.

UIKit because it's lightweight, I liked the look of it and wanted everything to have a consistent aesthetic, and because I didn't want to try and roll my own grid system in the time available.

## Regrets

With a detailed, finely broken down set of planned features, I would have preferred to test everything, but unfortunately, I was building the site out as I thought of new features (and frequently tweaking them), and didn't have a detailed development plan.

I also think it would have been super cool to have a map with markers for each of the restaurants linked to their Yelp pages.

## Spec

Use the Yelp! Api to retrieve data on restaurants

Allow users to search for restaurants by city

Allow sorting by price and rating

Display 20 restaurants at a time, with each linked to the yelp page for that restaurant

Any features beyond this are optional

## Optional features

Responsive design works on screen sizes from full desktop to tiny mobile

Dynamically updating page buttons, jump to page feature

Optionally query Yelp API for their highest rated restaurants in addition to sorting restaurants on the page by price and rating

Optionally query Yelp API with open-now and price filters

Site's graphics and icons adhere to Yelp's requirements as found here https://www.yelp.com/brand and here https://www.yelp.com/developers/display_requirements
