## Week One - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR.

1. What's the most useful thing you learned from completing the intermission week work?
* I think for me it was just learning general JS syntax. I was finally able to look at JS and it made some sense. Before this, it just looked like gibberish.

2. What are some tools to help debug JavaScript code?
* Debugger and console.log on the front end. Pry on the backend.

3. What are some tools you need in order to unit test your JavaScript?
* Mocha and Chai.

4. What is the syntax for invoking a function? Give an example.
* Adding parens after the function name. doAThing() vs just doAThing

5. What's `this` in JavaScript?
* I'm still a little fuzzy on this, but as far as I understand it, it's the execution context you're currently in.

6. What is Webpack and why is it useful?
* Webpack is an asset handler. It compiles the code into a single file, including CSS, and serves it.

7. When/why do you want to use event delegation?
* When you want dynamically updated content to have JS attributes attached to it. Like if you have an event listener on an element, but that element may dynamically update, the event listener won't be attached to that element if it's directly on that element. It needs to be on a parent element that will be present at page load.

8. What's `npm` and what do we use it for?
* Node package manager. It's basically like ruby gems for JS. It allows JS libraries to be loaded into a project.

#### Review  
9. What's the MVC design pattern? Describe each part of MVC.
* Model, view, controller. The model houses the logic, the controller handles requests/responses/routing/passing instance variables to views. The view renders what the user sees.

10. What are a few ways to optimize a Rails application?
* Caching, rewriting AR/SQL queries, background workers.
11. What's a background worker? When would we want to use a background worker?
* It's a way to send jobs to the background of the app if the result of that job isn't immediately needed. For instance, if a user updates something that isn't going to change what they see right now, a background worker can take in that task and make the update a little later. This keeps the app fast, because the user isn't waiting for server side logic to complete before a new page loads or a dynamic update of the current page happens. 
