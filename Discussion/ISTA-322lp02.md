--Lesson Plan 2

--ISTA-322

--Name: Xavier Kleiber


1. What is a controller? What does it do?  
 - They are responsible for responding to user input.

2. Explain the relationship between URLs and controller methods.  
 - The URL tells the routing mechanism which controller class to instantiate and which action method to call, and supplies the required arguments to that method. The controller's method decides which view to use.

3. What does it mean to say that, "The web is stateless?"  
 - The user vanishes and then is restored with every click.

4. Where in the directory structure of an ASP.NET MVC application do controllers live?  
 - The Controllers folder of the project.

5. What programming constructs do controllers contain?  
 - Controllers follow the basic class architecture and include methods also know as controller actions.

6. Where are action methods? What do they do?  
 - The methods inside a controller. An action method's job is to respond to URL requests, perform the appropriate actions, and return a response back to the browser or user that invoked the URL.

7. What are query parameters?  
 - Parameters passed via the URL.

8. How do action methods receive HTTP query parameters?
 - Passed in the URL as values assigned to named parameters.