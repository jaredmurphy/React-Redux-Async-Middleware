# React-Redux Async Middleware
A demonstration of how to write custom Redux middleware for use in async, promised-based action creators. Built with React, Redux, Axios, and Bootstrap.

#### The Problem with asnyc Redux actions

With vanilla Redux, we don't have any way to deal with an action whose payload is asynchronous in nature. Using the Axios library, we can make a request in the form of a promise. By the time the component renders, this promise has not yet been resolved. The promise is still waiting for the data when the action sends its payload to the reducer. 

#### Middleware solution 
This middleware can be found in `src/middlewares/async.js`

The middleware written for this app forces the promise to be resolved first and then sends the new payload back up the middlware tree, eventually sending the payload to the reducer which will update the Redux store.

Now, the Redux store is updated with the data we want, and the component renders its information correctly. 

#### Usage
- Clone this repo
- npm install
- npm start
- Go to localhost:8080
- See the correct data rendered on the page. 

#### Contribute
Fork, make changes, submit pull request.
