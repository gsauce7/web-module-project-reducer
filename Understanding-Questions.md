# Understanding Questions:
1. What are the steps of execution from the pressing of the 1 button to the rendering of our updated value? List what part of the code excutes for each step.
* The user presses the 1 button.
* 
...

 1. the onClick is invoked and the function runs the dispatch that calls the action

2. it finds addOne in ./actions/index.js where it needs to find what type:ADD_ONE  

3. it goes to  '../reducers/index.js' to find the case of ADD_ONE and sees that it updates state by spreading in  the old value of state, and saying that the value of the total: is state.total + 1

4. state.total shows up back on App.js where the totalDisplay value is now updated to show the previous number with 1 added to it

This of course is rendered to the DOM and displayed in the browser...

