1. How do we make flash messages display on a page?
They are called in the layout in an enumerable.
2. Where is cart information/temporary information usually stored?
In the session.
3. What might be some reasons not to store cart in our database? Are there any reasons why we would want to persist that information?
It would be extra space that is needed in the database. If a user just adds a bunch of stuff to the cart, then never comes back and buys it, we don't really want to store a record of that.
4. What is the purpose of the asset pipeline?
It precompiles CSS and JS assets in the rails app. It minifies them and compiles languages like coffeescript and sass into JS and CSS. It also puts all the JS and CSS assets into a single file each.
5. Why do we precompile our assets?
So that the files are as efficient as possible. If there is tons of whitespace, that takes unneeded processing to render.
6. What do each of the following tags do?

```ruby
<%= stylesheet_link_tag "application" %>
<%= javascript_include_tag "application" %>
<%= image_tag "rails.png" %>
```
The first links the CSS assets in the head of the layout so that the app has access to them on all pages.
The second does the same for JS.
The third will render an image in a view.

7. What are some of the elements of a great read me? What are some of the benefits of taking the time to update a readme for our project?
How to get the app up and running. How to log into the app. How to test, how to find the credentials for the app, who is the team that wrote the app, who to contact about the app, what are the dependencies.

It will make things a lot easier when it's been a while since we've looked at that app, or when another person or team looks at it.

8. What are the top four accessibility issues that we as developers should be aware of?

Cognitive, mobility, vision, hearing.

9. `before_save` is an example of a what? Where in our Rails application would we find a `before_save`?
It's a callback. It would be on a model.

10. Given the following object, how would we create a scope for all users who are active?

```ruby
User.create(name: "Happy", active: true)
```
scope :active, where(active: true)
11. What is the difference between a scope and a class method?
A scope is loaded every time the class is loaded, not when the method is called. I'm not really sure what the point of scopes is, to be honest. I read a bunch of blog posts about them, but I'm a little unclear what the advantage is over just writing a class method. 
