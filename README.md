Practice project for redux

Setup:
npm install redux react-redux
file directories in /src -
* /actions - files related to action creators
* /components - files related to components
* /reducers - files related to reducers
* index.js - sets up both the react and redux sides of the app

Notes:
Terminology
- Action creator, function that returns javascript object (action)
- Action, js object that has a type property and a payload
- Dispatch, creates copies of action and sends them off to reducers
- Reducers, essentially pieces of state
- State, compiled state

react-redux provides 2 components which connect both into react and redux
* Provider - Always has access to the store and keeps track of it, wrap your App in the Provider so the entire app has access to store
* Connect - Gives the redux store data to components through reacts context system and makes action creators available within the component, wrap the needed components with connect so it can communicate with Provider