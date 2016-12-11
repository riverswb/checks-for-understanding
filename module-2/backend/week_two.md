## Week Two - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!). 

Note: When you're done, submit a PR. 

1. At a high level, what is ActiveRecord? What does it do/allow you to do?
  * allows us to make SQL queries to a database by writing Ruby
2. What kind of methods are `belongs_to`, and `has_many`? (i.e. class or instance) Give an example.
  * Associations are class methods.
  ```ruby
  class Example < ApplicationRecord
    has_many :things
  end
  ```
3. What do they allow you to do?
  * associations allow us to use easier and more common methods.  To see what things the first Example has we could write Example.first.things
4. What's the difference between agile workflow and waterfall method?
  * Both break a large problem into stages.  Agile workflow is completing small pieces of each stage, then starting another piece.  Waterfall workflow completes stage 1, then 2, etc.  
5. What is the difference between `#new` and `#create`?
  * #new doesn't save.  #create is like #new & #save 
6. At a basic level, what does cURL allow you to do?
  * curl let's us see what is being trasfered back after sending a get request to the url you pass as an argument
7. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.
  * 1 Teacher --> Many Students
  * ![teacher student schema](http://i.imgur.com/aplbHrs.png)
8. Define foreign key, primary key, and schema.
  * foreign key: relates to primary key of related table
  * primary key: unique identifier
  * schema: the database, or a representation of it
9. Describe the relationship between a foreign key on one table and a primary key on another table.
  * the foreign key on one table points to the primary key on another table
10. What are the parts of an HTTP response?
  * status code, headers, body
11. Describe some techniques to make our Sinatra code more DRY. Give an example of when you would use these techniques.
  * DRY: don't repeat yourself.  If you have a few methods that have a similar part you can extract that part out to a new method, then call it in from those methods.  I used this style of DRY when making the weather conditions dashboard for Bike Share.

### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
2. Name your three favorite ActiveRecord rake tasks and describe what they do.
4. What can you expect from a group as you begin working together? As you continue working together?
5. What two columns does `t.timestamps null: false` create in our database?
6. What cURL flag can you use to send a `POST` request?
7. What case does JSON (and JavaScript) use for multi-word variables?
8. What case does Ruby use for multi-word variables?
9. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
10. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
11. Give an example of when you might want to store information besides ids on a join table.
12. Describe and diagram the relationship between patients and doctors.
13. Describe and diagram the relationship between museums and original_paintings.
14. What are some examples of acceptable values for the parts of an HTTP response?
15. What types of output do we want to test when we test our controllers?
16. What could you see in your code that would make you think you might want to create a partial?
17. Why might you use a helper method?
