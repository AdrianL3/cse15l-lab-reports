# **Lab Report 2**
***
#Part 1: Creating a Chat Server
//code image here

##Using `/add=message`  
//chat1 image  
**Which Methods in your code are called?**  
First, the `main` method is called and checks for a properly started server with the correct amount of arguments.  
Then the `start` method is called. Then `parseInt` is called and which is used to chain and call the `handleRequest` method. Within this method, the methods `getPath`, `equals`, `contains`, `getQuery`, and `split` are called.  
  
**What are the relevant arguments to those methods, and the values of any relevant fields of the class?**  
`main`: Takes the terminal arguments inputted by the user.  
  Sets `int port = args[0]` where `args[0]=2027`  
`start`: Has two arguments, with the first being `port` and the second being a new object of the `Handler` class.  
`handleRequest`: Takes a `url` object of type `URI`.  
`getPath`: takes no arguments  
`.contains`: In this case, the argument in this instance of calling the method is `.contains("add-message")`.  
`getQuery`: takes no arguments  
`split`: In this case, the argument in this instance of calling the method is `.split("=")` and `.split.("&")`.  
  `String[] parameters = {"s", "Hello%201%20am%20good&user", "swag"`  
  `String[] texts = {"Hello%201%20am%20good", "user"}`  
`equals`: In this case, the argument in this instance of calling the method is `.equals("s")`.  
localhost:2027/add-message?s=Hello%201%20am%20good&user=swag


Which methods in your code are called?
What are the relevant arguments to those methods, and the values of any relevant fields of the class?
How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.
