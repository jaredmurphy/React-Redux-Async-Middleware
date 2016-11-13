With vanilla Redux, we don't have any way to deal with an action whose payload is asynchronous in nature. With the Axios library, we  make a request in the form of a promise, and by the time the component renders this promise has not yet been resolved. By the time it hits the reducer, the promise is still waiting for the data. 

The middleware written for this app tells the reducer to hold off on updating the Redux store until the promise has been resolved. 

#Pleasant Ghost
Boilerplate that handles Node.js environment set up so you can start developing your front end NOW.

###What You Get
* React, React-DOM, React-Router
* Redux, Redux-Promise, Redux-Form
* Babel
* Webpack
* Axios
* jQuery
* Materialize
* Lodash
* Mocha
* Chai

###Usage
- Clone this repo
- npm install
- npm start
- Go to localhost:8080
- See your first working React component in action

###Contribute
Fork, make changes, submit pull request.
