--Lesson Plan 4

--ISTA-322

--Name: Xavier Kleiber


1. What is scaffolding?  
 - When you use a template to automate code generation. Think of the scaffolding of a building during construction.

2. What is a navigational property? What is a foreign key property?  
 - Used to navigate to the object using the dot operator.
 - Allows the object to be referenced from multiple database tables.

3. What is a virtual property? Why does the book use virtual properties?  
 - They give Entity Framework a hook into your plain C# classes and enable features such as an efficient change-tracking mechanism.

4. Explain eager loading. Explain lazy loading. What is the difference between the two?  
 - Eager tries to load all data using a single query. Lazy loading only loads the data for the primary object in the LINQ query, and leaves the other properties unpopulated.

5. What is meant by seeding a database? Explain.  
 - Let you to create some initial data for the application.

6. What is meant by the happy path? What is meant by the sad path? Give examples of each that are not in the book.  
 - It's code you execute when the model is in a valid state and you can save the object in the database. The sad path is the path the action takes if the model is invalid. An example of the happy path is when you ask for a phone number and they put in a valid one. An example of the sad path is when they leave the field blank.

7. In HTTP POST, what happens when action parameters are passed by the query request? What happens to the parameters and how are they expressed?  
 - When you have an action with a parameter, the MVC runtime uses a model binder to build the parameter. The default model binder can automatically convert and move values from the request into an object. In other words, when the model binder sees that an object has a Name property, it looks for a value named “Name” in the request. 

8. What is implicit model binding? Explain.  
 - Model binding implicitly goes to work when you have an action parameter. Sometimes the aggressive search behavior of the model binder can have unintended consequences. Occasionally there is a property you don't want (or expect) the model binder to set, and you need to be careful to avoid an “over-posting” attack. You use the Bind attribute to restrict the binding behavior.**

9. What is explicit model binding? Explain.  
 - You can explicitly invoke model binding using the UpdateModel and TryUpdateModel methods in your controller. UpdateModel throws an exception if something goes wrong during model binding and the model is invalid. Both methods have an override allowing you to specify an includeProperties parameter. This parameter contains an array of property names you're explicitly allowing to be bound.