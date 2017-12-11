## Week Two - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR.

1. What's one difference between ES5 and ES6?
* String interpolation is much better in ES6. You can do `String ${variable}` instead of "String " + variable

2. What's the difference between asynchronous and synchronous JavaScript?
* Asynchronous JS relies on the browser to give it an API that includes a queue. When a task has a callback, that task can be completed by the API, then have the callback added to the queue, then once the stack is empty, the callback will be added to the stack and run.
Synchronous JS just does one thing at a time. It completes one task, then does the next.

3. What are the four pillars of Object Oriented programming?
* Inheritance
* Encapsulation
* Abstraction
* Polymorphism

4. What are some tools available in JavaScript to help you write object oriented code?
* New syntax to create classes with encapsulated instance methods.
* Prototype inheritance.

5. What are some key concepts to be aware of when refactoring your JavaScript?
* What the specific code is doing. If it's responsibility is an AJAX call, an event listener, a response handler, or something else. Other than that, I feel like regular OOP standards: SRP, DRY, etc.

6. What's a callback function and what are some reasons when we use/need callback functions?
* A callback function is basically a nested function that is called when something else happens, and is used for asynchronous JS.

7. What are the different scopes of variables in Javascript? When would you want to define global variables?
* Global and local.
* We want a global variable when we need the variable in multiple contexts.

8. What's the difference between `==` and `===` in JavaScript?
* Loose equal vs strict equal. '==' will evaluate to true if the arguments can be coerced to be true.

9. Why do front end frameworks exist?
* The same reason any frameworks exist, to create an easier way to write an app.

#### Review  

10. Why do people say "HTTP is stateless"?
* Because there is no state as such passed in HTTP requests and responses. We can use cookies and sessions to emulate state.

11. Describe a RESTful API.
* An API that uses only the standard HTTP verbs (GET, POST, PATCH/PUT, DELETE), which give a uniform interface.

12. What are some main characteristics of a team following an agile workflow?
* Short sprints
* Frequent deployments
* Frequently updating requirements.
* An iterative approach.

13. What are some advantages **and** disadvantages to using OAuth to authenticate a user?
* It's easier to allow users to create accounts.
* It's easier to add user authentication into an app.
* With a service like LinkedIn there are API endpoints that are specific to a user, and need OAuth to access.

* The biggest downside to OAuth is that you don't have control over the flow of your user sign up or control over the information you can add as part of the sign up process. 
