## Express Exercises

In these exercises, you'll be asked to debug a few issues and add a few missing features in a sample Express application. We encourage you to use comments to explain any code you add or change, but you are not required to do so. The exercises are intended to take no more than 30 minutes each.

If you don't complete the exercises, please simply submit your partial solutions! :)

## Prerequisites / Expectations

These exercises are intended for someone that has ...
- Experience with Node and Express
- Has `npm` configured on their computer (to run the commands listed in "Setup")

## Setup

Open the project zip file that we sent to you along with these instructions on your computer. Once in the project directory, run npm install . to install all node modules.

To start your local server, run `npm start`. You should see the app running at `http://localhost:8080/`!


## Exercise 1 - Fruit Fixes

In this exercise, you will identify and resolve a number of issues related to the fruit endpoints. Follow the instructions for each issue below and resolve the relevant issue. Some of the endpoints may trigger a server error, which will need to be resolved.

### Issue 1 - Add Fruit
Send a POST request to the `/api/fruit/add-fruit` endpoint with the following body: `{"type": "orange", "color": "orange", "canEatSkin": false}`. You should receive a response containing a string containing a success message (eg. `New fruit added!`) and the new fruit object you added to the database. Make sure the fruit object matches this fruit object: `{type: 'orange', color: 'orange', canEatSkin: false}`.

### Issue 2 - Get Blue Fruits
Send a GET request to the `/api/fruit/blue-fruits` endpoint. You should receive a response containing an array of blue fruit objects (eg. `[{type: 'blueberry', color: 'blue', canEatSkin: true}]`)

### Issue 3 - Length of Color
Send a GET request to the `/api/fruit/grape` endpoint. Then, send a GET request to the `/api/fruit/apple` endpoint. You should receive the number of characrers in the fruit's color (eg. `6` for grape (purple)).

### Issue 4 - Get All Fruits
Send a GET request to the `/api/fruit/fruits` endpoint. You should receive a response containing an array of fruit objects (eg. `[{type: 'apple', color: 'red', canEatSkin: true}, {type: 'orange', color: 'orange', canEatSkin: false}]`).


## Exercise 2 - No Fruits After 10pm

Oops! We've decided we don't want our fruit GET endpoints accessed after 10:00pm. In this exercise, you will update the application so that if requests are made to any of our fruit GET endpoints after 10:00pm, a response is sent with the message "Go to sleep!"

## Exercise 3 - Version Vegetable

We've decided to add vegetables to our application! In this exercise, you will add new endpoints related to vegetables. Follow the instructions for each endpoint below.

### Endpoint 1 - Tasty Greens
Create an endpoint `/api/vegetable/tasty-greens` that returns all vegetables where `color = green` and `isTasty = true`.

### Endpoint 2 - Pairs With
Create an endpoint `/api/vegetable/pairs-with`. The endpoint should allow a user to send a request with the name of a vegetable that exists in the database, and a list of foods the vegetable pairs well with. For example, the request could include 'brussel sprout' and 'balsamic, bacon'. The endpoint should take the list of food and add it as an array property called 'pairsWith' to the relevant vegetable object in the database. For example, given the following vegetable object in the database: `{type: 'brussel sprout', color: 'green', isTasty: true}`, if the user sends 'brussel sprout' and 'balsamic, bacon' in the request, the response should contain something like: `{type: 'brussel sprout', color: 'green', isTasty: true, pairsWith: ['balsamic', 'bacon']}`.


## Submitting

Please zip/compress all files excluding the node_modules folder and email it to `kelsey@januaryadvisors.com and emi@januaryadvisors.com`.

Thank you very much for taking the time to participate! If you have any questions, feel free to email `kelsey@januaryadvisors.com and emi@januaryadvisors.com`.


