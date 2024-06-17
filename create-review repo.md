<b>CLONE REPO
$ git clone [path-to-repository-to-clone]</b><br>
NOTE:<br>
This command:<br>
<br>
takes the path to an existing repository<br>
by default will create a directory with the same name as the repository that's being cloned<br>
can be given a second argument that will be used as the name of the directory<br>
will create the new repository inside of the current working directory<br>
<br>
At this point, we have two Git repositories:<br>
<br>
the empty one that we created with the git init command<br>
the one we cloned with the git clone command<br>

<br>

<b>USE: git status</b>
<br>
It tells you what is happening inside git and git is understanding of our commands.<br>
run this command after every command.<br>
It improves your understanding of git and you will know your errors and which command to run next <br>
It tell us about new files that have been created in the Working Directory that Git hasn't started tracking, yet<br>
files that Git is tracking that have been modified<br>
<br>
<br>
<b>git log</b><br>
show info about all the commits till date<br>
By default, this command displays:<br>
<br>
+ the SHA<br>
+ the author<br>
+ the date<br>
+ and the message<br>
<b>git show</b><br>
show info about current commit<br>

+ --stat - to show the how many files were changed and the number of lines that were added/<br>
+ -p or --patch - this the default, but if --stat is used, the patch won't display, so pass -p to add it again<br>
+ -w - to ignore changes to whitespace<br>
<br>
<b>Navigating The Log</b>
<br>
to scroll down, press<br>
+ j or ↓ to move down one line at a time<br>
+ d to move by half the page screen<br>
+ f to move by a whole page screen<br>
+ to scroll up, press<br>
+ k or ↑ to move up one line at a time<br>
+ u to move by half the page screen<br>
+ b to move by a whole page screen<br>
+ press q to quit out of the log (returns to the regular command prompt)<br>
<br>
<br>
<b>$ git log --oneline</b><br>
This command:<br>
+ lists one commit per line<br>
+ shows the first 7 characters of the commit's SHA<br>
+ shows the commit's message<br>
<br>

<b>$ git log --stat</b><br>
This command:<br>
+ displays the file(s) that have been modified<br>
+ displays the number of lines that have been added/removed<br>
+ displays a summary line with the total number of modified files and lines that have been added/removed<br>
<br>
<b>$ git log -p</b><br>
This command adds the following to the default output:
<br>
+ displays the files that have been modified<br>
+ displays the location of the lines that have been added/removed<br>
+ displays the actual changes that have been made<br>
