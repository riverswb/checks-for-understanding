## Week Four Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

* What is a cookie?
* cookies are saved to a users browser to identify something about the user
* What’s the difference between a session and a cookie?
* sessions are encrypted, cookies are not
* What’s a flash and when do you want to use flashes?
* flashes are a message that is added to a page, it is useful to use flashes to let a user know if an action was successful or not
* Why do people say “HTTP is stateless”?
* because it never remembers anything about the user, that is why we use sessions and cookies
* What’s authentication? Explain.
* Authentication is the process of a user logging in to an account, ensuring that the password supplied matches whats in the database
* What’s the difference between authentication and authorization?
* authorization is what pages/ functionality a user is able to access. Authentication is logging a user in or not.
* What’s a before filter?
* like a list of things for a controller to do before finding the method
* How do we keep track of a user once they’ve logged in?
* sessions

* When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?
* namespace a resource when the type of authorized user will need access to a lot of aditional functionality or different views, nest if the users will only need slightly different functionality or views

* At a high level, what tools can you use to implement authorization? How would you use them?
* Bcrypt
* What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?
* enums can be used to create a default value for a column, the data type needs to be integer
* What are some strategies you can use to keep your views DRY?
* partials 
