## Week Three Recap

### Instructions
Fork this repository. Be sure to pull the latest changes to your local repo. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

1. What is the entry at the command line to create a new rails app?
  * rails new "name"
2. What do Models generally inherit from in rails?
  * ActiveRecord::Base
3. What do Controllers generally inherit from in a rails project?
  * ApplicationController
4. How would I create a route if I wanted to see a specific horse in my routes fitle assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?
  * resources :horses, only: [:show]
5. What rake task is useful when looking at routes, and what information does it give you?
  * rake routes: gives the prefix for the path, type of request, url, controller#action
6. What is an example of a route helper? When would you use them?
  * horses_path.  Use them to route to specific pages
7. What's the difference between what `_url` and `_path` return when combined with a routes prefix?
  * _path returns relative url, _url returns the whole url
8. What are strong params and why are the necessary?
  * strong params is how we verify that only allowed information is being sent to the database
9. What role does `form_for` play in helping us create our forms?
  * form_for is a helper that makes it easy for us to make forms using helper methods
10. How does `form_for` know where to submit the user's input?
  * from the arguments passed to the form_for
11. Create a form using a `form_for` helper to create a new `Horse`. 
  ```ruby
  <%= form_for @horse do |f| %>

  <%= f.label :name %>
  <%= f.text_field :name %>

  <%= f.label :age %>
  <%= f.number_field %>

  <%= f.label :location %>
  <%= f.text_area :location %>

  <%= f.submit %>

  <% end %>
  ```
12. Why do we want to validate our models?
  * to ensure critical information is included, that fields are unique if necessary
