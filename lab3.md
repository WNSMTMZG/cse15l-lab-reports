##Lab report 3: String Server

#Building the String server:

* The StringServer codes are as follow:
 ![image](https://user-images.githubusercontent.com/103611867/215676264-34fec104-b946-4eff-a112-e6e13b317751.png)
* enter the following command into the terminal, and then click on the following link to access the server page:
 ![image](https://user-images.githubusercontent.com/103611867/215676543-d837acf3-bfc1-44de-8c0a-f607e4048a69.png)
* First, a welcome message will be displayed with instructions give on how to add message
  ![image](https://user-images.githubusercontent.com/103611867/215676680-0fc6a710-b3ed-44e4-ad89-f19dd8934733.png)
* Then, input the following line of code: add-message?s=Hello to access Hello
  ![image](https://user-images.githubusercontent.com/103611867/215677118-9bc37e1e-dfdd-4d99-a8a9-9bd48c4be9b9.png)
  * The method handleRequest is called
  * The relevant arguments are the parameters (url), the instance variable(defaultstring), as well as our added input(parameters[])
  * The value of our instance vairble is defaulted to empty "". However, we will concatenate our input to the string everytime we run /add again.
  * The value of parameter will change everytime we input a new string. This iteration would be string"Hello"
* Then, input the following line of code: add-message?s=How are you
  ![image](https://user-images.githubusercontent.com/103611867/215678678-a6b8de07-044c-4444-9b9f-f9b5bbbc4686.png)
  * The method handleRequest is called again
  * The relevant arguments are the parameters (url), the instance variable(defaultstring), as well as our added input(parameters[])
  * The value of our instance variable defaultstring is now changed to "Hello", then after concatenating it with "How are you", the defaultstring is now "Hello"\n"How are you"



