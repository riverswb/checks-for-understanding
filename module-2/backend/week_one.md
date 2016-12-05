## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

1. List the five common HTTP verbs and what the purpose is of each verb.
    * get: receive from server
    * post: send to server
    * put: for uploading
    * delete: Deletes stuff
    * patch: not sure, read about it in mod 1
2. What is Sinatra?
    * a domaign specific language. "Baby Rails"
4. What is MVC?
    * Model View Client. Archetecture used by rails that we imitate in Sinatra
5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
    * So that people working with us know how to read what is happening
6. What types of variables are accessible in our view templates without explicitly passing them?
    * ivars
7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?
  
  ```ruby
  get '/horses' do
    @count = 1
    name = "Mr. Ed"
    erb :index, :locals => {:name => name}
  end
  ```

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed`?
9. What's the purpose of ERB?
    * Embedded Ruby, let's us use html and ruby in the same file.
10. Why do I need a development AND test database?
    * Development DB is for all of the data (or a representative sample) that will be used in production.  Test DB is separate so that you are saving and deleting from the development db
11. What's responsive design?
    * A website / app should adjust based on the user
12. What is CRUD and why is it important?
    * Create, Read, Update, Destroy.  How we interact with our code / app.
13. What does HTTP stand for? 
    * Hyper Text Transfer Protocol
14. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
    * <%= code => : runs the code and shows the outcome
    * <% code %> : runs the code
15. What's an ORM?
    * ActiveRecord is an ORM.  it is written in an object oriented language and wrapped around a relational database
16. What's the most commonly used ORM?
    * I have no clue
17. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
    * get '/restraunts': see all restraunts
    * get '/restraunts/:id': see specific restraunt
    * get '/restraunts/new': see form to create new restraunt
    * get '/restraunts/:id/edit': see form to update horse
    * post '/restraunts': submit to save new restraunt
    * put '/restraunts/:id': submit to update restraunt
    * delete '/horses/:id': delete a restraunt
18. What's a migration? 
    * instructions to modify a database
19. When you create a migration, does it automatically modify your database?
    * nope, gotta run the migration (rake db:migrate) to modify
20. How does a model relate to a database?
    * ? We can model how we plan to connect tables in out database with keys and foreign keys by either writing it out, using software, or online resources.  
21. What's the difference between agile workflow and waterfall method?
    * agile cuts slices from the many steps of a project so that you continously work on the traditional steps
    * waterfall is the traditional steps method, finsh one step and move to the next
22. What is the difference between `#new` and `#create`?
    * new does not save, create is like "new & save" in one step
