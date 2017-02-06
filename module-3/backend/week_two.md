## Week Two - Module 3 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!). 

Note: When you're done, submit a PR. 

* What's OAuth?

Oauth is standard protocol for authorizing a user through another service.
* What are some advantages/disadvantages of implementing OAuth?

Pro & Conn: security handled by someone else.
* How many exhanges of information need to take place before a user is authenticated with OAuth?

2
* Why do we want to create services?

To communicate with outside data sources and keep controllers DRY
* Why is it good practice to create PORO's with the data received from an API?

We wrap services with POROs to help with DRYness and to reduce the amount of ivars sent to views.
* What do we use VCR for? Why is a good idea to use this tool?

We use vcr to record the information returned from an api call.  It is good to prevent api use charges, when you may not have internet connection.
