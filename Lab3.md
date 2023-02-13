## lab report 3 

# The keyword I decide to research is grep
* The first grep command I'm looking for to use is grep -r "String args":
  1. Function: look through the current folder and find all files that contains the following string(or input)
  2. Pratice output: When I try to look for txt files inside written_2 that contains the string "Athens", this is the given output:
    * <img width="995" alt="image" src="https://user-images.githubusercontent.com/103611867/218586425-75ada98c-2bb4-41af-b4ac-4a18b61dfe35.png">
    * <img width="698" alt="image" src="https://user-images.githubusercontent.com/103611867/218590867-d4f8fce2-e2e7-402a-ad86-8c0f1690a15d.png">
    * and off course, there are a lot more as I can't only screenshot a limited amount
  3. Source: I already know this from before

* The second grep command I'm looking for to use is grep -r -c "String args":
  1. Function: this will count the number of inputs contained in each files of my current repository/folder:
  2. practice out: This is what I get when I input that command:
    * <img width="655" alt="image" src="https://user-images.githubusercontent.com/103611867/218588179-5798493d-eda9-4d92-a724-906d356294af.png">
    * <img width="573" alt="image" src="https://user-images.githubusercontent.com/103611867/218590759-593148fe-6735-4545-a33d-a3d9bfeec84d.png">
    * the output shows that I have 12 word strings inside HistoryGreek.txt, and one result inside HandRHawaii.txt, which is the intended result
  3. Source: https://www.hostinger.com/tutorials/grep-command-in-linux-useful-examples/#:~:text=Grep%2C%20or%20global%20regular%20expression,any%20lines%20that%20contain%20it.

* The thid grep command I'm looking for to use is grep -n [String args] file:
  1. Function: find the lines that contains certain string characters in the file and display which line has it
  2. Practice output: 
    * <img width="511" alt="image" src="https://user-images.githubusercontent.com/103611867/218589598-55746b47-3b6b-4bf7-8d6a-94e9a6e8d719.png">
    * <img width="533" alt="image" src="https://user-images.githubusercontent.com/103611867/218590527-5f7ab448-4677-473c-b5d3-21b10b3814fd.png">
    * As the output has displayed, the lins that contained word "the" are line 7,8,15,18,20,22| The lines containing "Hong Kong" are line 7,10,19,15
  3. Source: https://www.hostinger.com/tutorials/grep-command-in-linux-useful-examples/#:~:text=Grep%2C%20or%20global%20regular%20expression,any%20lines%20that%20contain%20it.

* The fourth grep command I'm looking for to use is grep -vn [String args] file:
  1. Function: this is like the reverse operation of the last one, it will printout lines that doesn't contain the above character
  2. Practice output: when I did invert search the, here are the outputs:
    * <img width="628" alt="image" src="https://user-images.githubusercontent.com/103611867/218590204-6d9fd1a9-937d-49cb-a016-6f556b8fd576.png">
    * <img width="712" alt="image" src="https://user-images.githubusercontent.com/103611867/218590396-63f57620-81be-4de4-9fc5-02c04219a44f.png">
    * So, it printed out characters that doens't have the character "The" and "Hong Kong"
  3. Source: https://www.hostinger.com/tutorials/grep-command-in-linux-useful-examples/#:~:text=Grep%2C%20or%20global%20regular%20expression,any%20lines%20that%20contain%20it.


  
