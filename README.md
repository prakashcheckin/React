# React

npx create-react-app my-app

npm i react-router-dom

npm i redux react-redux redux-thunk

npm install react-router-dom react-fontawesome react-simple-sidenav react-slick --save


const { id } = this.props.match.params; => this line fetch the ID data from the url

preventDefault : 
asyn: Javascript basically a synchronse and single thread program. async will work that method in asynchronse way.


componet name always should be in caps



context api:

create a Provider
Provider hold the state of the application
To share the values in the Provider we need a context. To create a context, use create context.
once context created, export the context and with help of context return the poducer.


if the method is created inside a class, then that method should be called with help of this.
setstate only allow single line  arrow function


Life cycle of component: render and componentDidMount methods are component lifecycle method. these are not arrow funcionts



Redux:
Step 1: create all the content in store. In store file import the reducers. 
Step 2: get Provider and store in app.js. and pass the store inside the Provider
step 3-a: Create Reducers folder and Index.js inside the reducer is a meeting place for all reducers. so get combineReducers from redux.combinereducer will be called with
		parameter of object. that object key(contact) will be anyname and value will be all the Other reducers(contactReducer).  
		Object key wil be used entire application to fetch the state.
step 3-b: Create contactReducers.js and do the logics
Step 4: if we want to use state in any of the component(Contacts), we need connect function. connect function get two parameter.
		first parameter is mapping state to props of that compontent(Contacts).
		Secont parameter is dispatch action.
