## Week Three - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR.

1. At a high level, what is Node?
* It's a JavaScript runtime environment. It uses the V8 engine to run JS on the server side.

2. What is Express? What is Express similar to in the Ruby world?
* A lightweight framework for JS. It's kind of like Sinatra.

3. How do we setup a route when creating an API with Node and Express? Please provide a code snippet.
* app.get('/api/v1/foods', someFunction).

4. What do we use Knex for?
* For making DB queries.

5. How **could** you organize your code to follow the MVC design pattern in your Quantified Self project?
* POJOs(models)
* Controllers(define routes routes)
* Views(appending HTML)

6. How do you execute raw SQL in node?
* return database.raw('SQL QUERY')

7. What are some advantages to having your front end and back end code live in separate applications? What are some disadvantages?
* It keeps things clean. We can use each app specifically for what it's good at.
* There can be some issues with CORs and other communication between the apps.

#### Review  

8. Describe DNS.
* Resolves the domain name into an ISP address.

9. What does writing clean code mean to you?
* Having concerns separated out into logical components. Having SRP enforced throughout. There's a lot here. I feel like clean code can mean a lot of things, but you know it when you see it.

10. If you were building an application that models hotels, what classes would you need? What classes would be responsible for what functionality? Hint: think about what tables you would need in the database, how those records would relate to each other, and good OOP.
* Hotel class. This would be a larger parent class. has_many rooms. has_many guests
* Room class. belongs_to hotel. has_many reservations
* Reservations class. belongs_to room.
* Guests. has_many reservations, has_many rooms through reservations.
