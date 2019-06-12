# Aesthetics Pro Testing Server


[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Welcome to the AP Testing challenge - this is a simple way to see how you write code and consume a simple endpoint. This challenge will help us see you demonstrate the following:

  - Your basic coding practice
  - Can you consume an endpoint given some credentials
  - Can you use a web response to do something meaningful.

### First Step!
This is your initial setup for the challenge so go ahead do the following:

  - Create three files: "index.html", "style.css", "action.js"
  - Link your files together within your basic html document (nothing crazy yet).
  - We're gonna set this aside for a moment and get to the next part.

### Challenge #1 (AP Secret)

You'll be consuming and creating many endpoints here at Aesthetics Pro, so we'd like to see how you handle getting some data. This challenge will see how you handle credentials when writing a GET request to a given endpoint.

-First, within your action.js file, create a function that hits the following endpoint:

     https://ap-testing.herokuapp.com/secret

-You may notice that if you fail to provide any authorization headers, (i.e. creds) you won't be able to get the secret.

Here are your credentials (we hope you use a better password in real life):
* Username: `apTestUser`
* Password: `apIsAwesome1234`

-To best complete this exercise, you need to remember to properly set your request headers (hint hint). The server is expecting this exact username and password from you. The server will only accept a request with headers that have an 'Authorization' property on it in the following format: 
- `'Basic username:password'`

*Note you have an option here of just using a CLI-based tool to make this request (curl or HTTPIE). If you choose to do so, please document how you went about doing so.

If you've gotten the secret, go ahead and document that somewhere or leave the function inside your JS file that logs it to the console, your choice.

### Challenge #2 (Using the Data)

The next challenge builds on what you just did in the last one. This time you'll be getting some JSON back that has some specifications for you to use. We're going to have you display the specs you get back as actual styled markup.

-Now, within your action.js file, create a function that hits the following endpoint:

     https://ap-testing.herokuapp.com/data

-**NOTE You will still need to have an authorized request, same as the last challenge!

-Once you've gotten a proper response, you should receive a JSON object that specifies three objects for you to 'create' inside your markup file. Make sure your function logs this to the console.

##### Instructions for creating your objects:
- Create a dom representation for each 'object' with the right color.
- Make sure the 'name' property displays in the center of your object.
- Make sure you create the right quantity of objects specified.
- Also make sure to size each object (with each respective quantity) as specified.

-This shouldn't take very long to create, we just want to see how you style your markup and your basic coding practices.

*BONUS*: if you so choose, you can show off your wicked-awesome frontend skills by animating or styling the heck out of your 'objects.' Not totally necessary though.

### To Submit:
- Upload your three files to a github repo where we can pull it down and run locally.
- Please make sure you've got some documentation explaining your process and why you did things. Feel free to use jQuery or a similar framework to help you make the GET requests.
- Log your answers to the console so we can see that you're consuming the endpoint properly. (There should be two differnt answers, one for each challenge. Just log the response of the endpoint)
 
- GOOD LUCK!
