## Lab report 3: String Server

# Building the String server:

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
  * The value of parameters is now"How are you" and will be added to defaultstring to update our instance variable

# Identifying the bug

The bug I decide to choose is from reversed method from arrayexample class
* The failure inducing input:
 ```
# code block
@Test
  public void testReversed1() {
    int[] input1 = {1,2,3};
    assertArrayEquals(new int[]{3,2,1}, ArrayExamples.reversed(input1));
  }
   ```
we see there is a error message displayed, and of course, since our implementation of the reverse method is wrong, the test would not pass
    ![image](https://user-images.githubusercontent.com/103611867/215684242-5fe4680d-76cc-4b67-8d3a-aaf964e4b319.png)

* The only input that doens't result in a failure is when our arraylist is empty

 ```
# code block
  @Test
  public void testReversed() {
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  }
 ```
This will not result in a failure as we basically didn't need to manipulate anything for an empty arraylist, let alone reverse it. So the test is passed
    ![image](https://user-images.githubusercontent.com/103611867/215684790-18cd4730-721e-464d-a6de-b649d2ef2724.png)

* Running the Junit test:
   ![image](https://user-images.githubusercontent.com/103611867/215685142-c7c299f0-2bb6-462b-b10c-f713ed3e0c9b.png)
    We see that the first test passed for input that doesn't induce a failure, and the second and third test failed for failure-induced input
    
* Fixing the bug
* before  

```
# code block
   static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
```
 
 
* after
```
# code block
 static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
```
 * Explanation: there are couple mistakes
    * returned arr instead of newArray
    * we need to concatenate the element from the old array into the new array
    * arr would be an empty array after running the for loop because the newArray is initalized to be empty
 
 # Things learned
 
 * The thing that struck me the most is creating a server, this is very interesting, that not only do I get play around after I built my server, the building process itself is very entertaining. I get to think about what to put into where and what argument do I need to pass in for it to work. The junit testing I'm already pretty familiar from before, but it nice to get practice at it again. OVERALL GREAT LAB!!!
    
