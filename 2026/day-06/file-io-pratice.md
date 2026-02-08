# Back to  fundamentals. Learning file Input Output in linux

1.)"touch notes.txt" :- This creates a new text file.
2.)"vi notes.txt" :- Vi here stands for visual editor and it opens a text editor where we can enter all the text we want
3.)"cat notes.txt" :- cat command is used to view the contents of the file
4.)"echo "adding new line" >notes.txt" :- This command deletes all the existing content and adds the line that is mentioned in this particular command 
5.)"echo "append redirection" >>notes.txt" :- This command appends the line to the existing file.
6.)"head notes.txt" :- displays the first 10 lines from the file
7.)"tail notes.txt" :- displays the last 10 lines from the file 
8.)"echo "checking how tee works" | tee -a notes.txt ":- This command appends the new line to the text file and displays only the line that is getting appended.