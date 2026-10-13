Day 06 – Linux Fundamentals: Read and Write Text Files
Objective
Practice creating, writing, appending, and reading text files using basic Linux commands.
Commands Practiced
1.	touch notes.txt — Created an empty file.
 
2.	echo "Line 1: Learning Linux file operations" > notes.txt — Wrote the first line using redirection.
 
3.	echo "Line 2: Practicing output redirection" >> notes.txt — Appended the second line.
 
4.	echo "Line 3: Using tee to write and display" | tee -a notes.txt — Appended and displayed the third line.
 
5.	cat notes.txt — Displayed the complete file.
 
6.	head -n 2 notes.txt — Displayed the first two lines.
 
7.	tail -n 2 notes.txt — Displayed the last two lines.
 
8.	wc -l notes.txt — Counted the lines in the file.
 
Key Learnings
•	> creates or overwrites file contents.
•	>> appends content without removing existing lines.
•	tee -a displays text and appends it to a file.
•	cat, head, and tail help read complete or partial file contents.
Result
Successfully practiced basic Linux file input/output operations and verified the contents of notes.txt.


