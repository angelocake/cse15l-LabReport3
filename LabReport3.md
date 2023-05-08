# Lab Report 3

## Researching Commands (`grep`)
* The command alterations that I chose to further reseach on for grep were as follows:
  1. `-n`: displays the lines that matched the input and the line number they were found on
  2. `-c`: displays the number of lines that match the given input
  3. `-l`: displays files containing the matched input
  4. `-o`: displays the matched pattern only
  5. `-v`: displays all lines without matches to the input
(Note: the following commands need to be run in a terminal with bash installed)
## `-n`
* This command displays the lines that matched the input and the line number they were found on
* To write the command you need to follow this format: `grep -n "text you are looking for" filename/path_to_file`

Here is one example of me using the command `grep -n`
![example_n_1](https://user-images.githubusercontent.com/130005453/236670082-91ed1bd1-736e-4f3a-b561-0d1fe276b86f.png)
* Above is an example in which I used the `grep -n` to firgure out which lines the word "case" apears in on a file called chapter-1.txt
* The blue arrows point exactly where the word "case" appeared in the text
* The green arrows point out the line numbers which contained the word "case"
* The red bracket is to show a small portion of the actual file in which shows the line and points out a single instance on where the word "case" is found

Here is another example of me using the command `grep -n`
![example_n_2](https://user-images.githubusercontent.com/130005453/236669812-7098e9f4-2b46-4431-bbd3-27c018b3a2bb.png)
* Above is an example in which I used the `grep -n` to firgure out which lines the word "solve" apears in on a file called chapter-1.txt
* The output of this terminal is a print out of a single line from the chapter-1.txt file which contained the word "solve" with its respective page number
* The blue arrows point exactly where the word "solve" appeared in the text
* The green arrows point out the line number which contained the word "solve"
* This 

These example illustrate the key use of the command `grep -n` which is used when trying to search through a large txt document to find specific instances. To make it better, it also displays the line that the instance was found on making it easier to search through a document for that instance of the match.

## `-c`
* This command displays the number of lines that match the given input in a file
* To write this command you would follow this format: `grep -c "text you are looking for" filename/path_to_file`

Here is an example I ran for the command `grep -c` which I checked the line count that had the word "case" in it in the file chapter-1.txt
![example_c_1](https://user-images.githubusercontent.com/130005453/236668771-ab3c64a0-505b-4d1f-bc75-524b6528f8f9.png)
* The red bracket portion is the example terminal which I used the `grep -c`command
** It's output was the number 3, meaning that within the chapter-1.txt file, there are only 3 lines which contain the word "case"
* The blue bracket is to show you which lines the word "case" is found in and the specific place in that same sentence where the word is found.

Here is another example I ran for the command `grep -c` which I checked the line count that had the word "state" in it in the file chapter-1.txt
![example_c_2](https://user-images.githubusercontent.com/130005453/236669531-0c707fa0-feed-4003-a47f-d3b54549dc79.png)
* The red bracket portion is the example terminal which I used the `grep -c`command
** It's output was the number 10, meaning that within the chapter-1.txt file, there are only 10 lines which contain the word "state"
* The blue bracket is to show you which lines the word "state" is found in and the specific place in that same sentence where the word is found.

From these examples you get the idea of why you would want to use this command in order to see the number of instances of a specific word. It also comes in handy when combining that piece of information with the command `grep -n` because this command gives you more specifics on more than just the number of instances that the word is found.

## `-l`
* This command displays the files conatining a match with the input
* To write this command you would follow this format: `grep -l "text you are looking for" filenames/path_to_file`
(Note:For optimal use I would put a path and end with `*.txt` to see which files in the directory have the match)

Here is an example I ran in the command `grep -l` which I checked the 911report directory for all the files that had the word "tech"
![example_l_1](https://user-images.githubusercontent.com/130005453/236739301-b96267d0-f40c-4ef8-af9f-00f892697b2e.png)
* The image above actually has two examples of the command running
  1. The first command labeled "1)" (in red) is me running the `grep -l` command searching the directory for "tech"
      * The terminal output in this section is a ton of file names which had a word that matched "tech"
      * To verify that it was not all the files, in the left of the image, you are able to see all the file names of the 911reports directory
      * Not all of them are present on our list in the terminal so not all of them have some word that has "tech" in it
  2. The second command labeled "2)" (in red) is me running the `grep -l` command searching the directory for "techmical"
      * The terminal output in this section is an empty output
      * Nothing was shown because no words in any files in the 911reports directory have the word "techmical" in them


Here is another example I ran in the command `grep -l` which I checked the 911report directory for all the files that had the word "cases"
![example_l_2](https://user-images.githubusercontent.com/130005453/236739449-8db85ac6-96c3-4b0a-8598-1dd5814865c7.png)
* The image above shows me running the command on my terminal and the computer returning back serveral file names found in the 911reports directory
* All of these files that were shown have the word "cases" somewhere in them, hence why the computer printed out only these files rather than all files in the 911reports directory

From the three example cases above, we get the understanding that this command option can be used when searching a file for a specific piece of information. It's also helpful in searching an entire directory worth of files because it will return all files which have a word in them that matches the input we gave.

## `-v`
* This command displays all the lines that don't match the given input
* To write this command you would follow this format: `grep -v "text you are looking to exclude" filename/path_to_file`
(Note: If there is a lot of information in a file, specific inputs usually result in a lot being printed back out)

Here is an example I ran for the command `grep -v` which I checked the lines that didn't have the letter "i" in it for the file preface.txt
![example_v_1](https://user-images.githubusercontent.com/130005453/236737925-18fdf87d-9118-4127-85e6-bf9d8b5d0c37.png)
* The output of the command that I ran were a total of 4 lines of text from the preface.txt file
* If you read through the lines returned, you'll see that none of the lines contain an "i" in them
* To prove that the lines that were printed were only those without an "i", you can see a green arrow pointing to the line number 103
** There is also a command ran at the end which is used to display the number of lines in the preface.txt file that contain the letter "i"
** If there are a total of 103 lines in the document and 99 of the lines contain the letter "i" then only the 4 lines that were printed in the `grep -v` command are the only lines that don't contain the letter "i"

Here is an example I ran for the command `grep -v` which I checked the lines that didn't have the letter "o" in it for the file preface.txt
![example_v_2](https://user-images.githubusercontent.com/130005453/236738630-3ce140f4-ff1c-4bf7-8e1c-eb932ea31e85.png)
The output of the command that I ran were a total of 3 lines of text from the preface.txt file
* If you read through the lines returned at the bottom of the image, you'll see that none of the lines contain an "o" in them
* To prove that the lines that were printed were only those without an "o":
** Thee command `grep -c` which is used to display the number of lines in the preface.txt file that contain the letter "o" which is 100 lines
** If there are a total of 103 lines in the document and 100 of the lines contain the letter "o" then only the 3 lines that were printed at the bottom of the image are the only lines that don't contain the letter "o" in them

These example code pieces should give you the understanding that this command is interesting to find out which lines in a text don't have a specific character/word. Although I didn't put a word for y example, it is still possible to do so and get lines returned that would represent sentences from preface that don't contain the word. In this sense, the command could also be applied to several files at once to do a mass search for the files that may be lacking a certain word/phrase.

## `-o`
* This command displays all the portions of text taht match the given input
* To write this command you would follow this format: `grep -o "text you are looking to match" filename/path_to_file`
(Note: if the input occurs a vast number of times in a file then it will be printed a vast number of times)

Here is an example I ran for the command `grep -o` which I checked the number of matched for the word "case" in the file chapter-1.txt
![example_o_1](https://user-images.githubusercontent.com/130005453/236736410-6cdaba12-3a83-45a0-84a3-d4c40df5561e.png)
* The middle part of the terminal (with a 3 next to it) is the example code I ran to demonstarte the `grep -o` command
* The output in this part was a print out of the word "case" 3 times
** The reason for this was because the instance of "case" was found 3 times in the file chapter-1.txt so the word "case" was printed three times
** To prove this, the bottom part of the terminal shows a `grep -c` code being implemented to seaarch for the number of lines which had the word "case" in it for the same exact file as the middle command
*** Since the number of times the word "case" was the exact same number of lines which had the word "case" in it then we can assume that the command `-o` prints the input the number of times corresponding to the number of times it was found in the document.

Here is an example I ran for the command `grep -o` which I checked the number of matched for the word "tech" in the file chapter-1.txt
![example_o_2](https://user-images.githubusercontent.com/130005453/236736984-1a409403-b8a0-43c2-8875-ecac1ff15614.png)
* The output in this terminal was a print out of the word "tech" 3 times
** The reason for this was because the instance of "tech" was found 3 times in the file chapter-1.txt so the word "tech" was printed three times
** To prove this, a control+f was done on this programm in which I searched for the number of instances of "tech"
*** On the top right of the image you can see that the "tech" has 3 total instances in the document
* So because "tech" was found 3 times in the document chapter-1.txt it was printed in our terminal 3 times as well

So the command(`grep -o`) seems to be useful for finding the number of instances a certain word/phrase appears in a `.txt` file. It is also worth mentioning that the command itself only find instances that the certain word/phrase appears but does not print out the word it came from in the text. So if you were searching for "tech" in a file, you would see tech printed a certain number of times because it was found in words such as "technology". It's also worth noting that the command `grep -n` basically has the same functionality without having to print out the input phrase a certain number of times.

# Site used for information
[geeksforgeeks.org](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)
