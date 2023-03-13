## Lab report 4, reproducing competition

I. Step 4(Log into ieng6):
* <img width="581" alt="image" src="https://user-images.githubusercontent.com/103611867/224833798-36679eee-49f3-4f2b-9e13-96fbd5eed5f3.png">
* Enter the username, there should not be any password this time since we've alreay set up an SSH key 


II. Step 5

* Since we already have a lab7 folder, we need to remove it first, use command `rm -rf la`
  * ![image](https://user-images.githubusercontent.com/103611867/224835235-eaf1f407-b1fe-4b5c-bcab-e7d1c8ba4b5e.png)

* Second, I git clone the repository to my ieng6 account, use git clone, make sure to copy the ssh link not the http link `<enter>`
<img width="570" alt="image" src="https://user-images.githubusercontent.com/103611867/224840545-cd326070-7c97-4ddf-a281-b5b1437e06ef.png">


III. Step 6
* Now we need to run the test: 
* The key I used were: `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` and `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests`. It failed one test and the result are the following:
* <img width="856" alt="image" src="https://user-images.githubusercontent.com/103611867/224836582-c169f9d7-c40e-4a35-a4c0-afc1d582786f.png">
* It's throwing a test timed out exception after 500 millisecond 

IV. Step 7
* Now we need to edit the code to fix it:
* Use command `nano ListExamples.java`
* Then I used the command `Ctrl W while(index2 < list2.size()) <down> <down> <right> <right> <right> <right> <right> <right> <right> <delete>2` to fix the error (The error we need to fix is index1 should be index2 in the while loop with index2< list2.size
* Then we need to save the java file: `Ctrl O` and then `Ctrl X` to exit 

IIX. Step 8
* Now we need to run the test and show that they all pass: 
* Key pressed: `<up> <up> <up> <Enter> <up> <up> <up> <up> <Enter>`
* <img width="853" alt="image" src="https://user-images.githubusercontent.com/103611867/224839010-988ac9e2-0c69-4d42-8295-5e7edf49cf1c.png">
* The message shows that all test passed

IX. Step 9
* Finally we need to commit and push the change to Github
* Command used: `git add ListExamples.java, git commit -m "fixed", git push`
* <img width="734" alt="image" src="https://user-images.githubusercontent.com/103611867/224842332-19f9b6d0-e5c0-469c-a01b-ddd6b95f274c.png">
* for this, I just inputed the command above manually, there is no up or down scrolling. 
* Finally, it is pushed







