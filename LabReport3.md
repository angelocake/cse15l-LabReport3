# Lab Report 3

## Researching Commands (`grep`)
* The command alterations that I chose to further reseach on for grep were as follows:
  1. `-n`: displays the lines that matched the input and the line number they were found on
  2. `-c`: displays the number of lines that match the given input
  3. `-l`: displays files containing the matched input
  4. `-o`: displays the matched pattern only
  5. `-v`: displays all lines without matches to the input
(Note: the following commands need to be run in a terminal with bash installed)
### `-n`
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

### `-c`
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

### `-l` (files containing the match)
* 
![example_l_1](https://user-images.githubusercontent.com/130005453/236739301-b96267d0-f40c-4ef8-af9f-00f892697b2e.png)

![example_l_2](https://user-images.githubusercontent.com/130005453/236739449-8db85ac6-96c3-4b0a-8598-1dd5814865c7.png)


### `-v` (all lines without matches)
* 
![example_v_1](https://user-images.githubusercontent.com/130005453/236737925-18fdf87d-9118-4127-85e6-bf9d8b5d0c37.png)

![example_v_2](https://user-images.githubusercontent.com/130005453/236738630-3ce140f4-ff1c-4bf7-8e1c-eb932ea31e85.png)


### `-o` (matched pattern only)
*
![example_o_1](https://user-images.githubusercontent.com/130005453/236736410-6cdaba12-3a83-45a0-84a3-d4c40df5561e.png)

![example_o_2](https://user-images.githubusercontent.com/130005453/236736984-1a409403-b8a0-43c2-8875-ecac1ff15614.png)

# Site used for information
[geeksforgeeks.org](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)
