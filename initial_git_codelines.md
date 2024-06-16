ssh key paraphase:riya8866<br>
<b>start:</b><br>
1.git init<br>
2.git add README.md<br>
3.git commit -m "first commit"<br>
4.git branch -M main<br>
5.git remote add origin git@github.com:riya8866/git.git<br>
<br>
6.git fetch origin master:tmp               <b>(master can alse be named as main)</b><br>
7.git rebase tmp<br>
8.git push origin HEAD:master              <b>(master can alse be named as main)</b><br>
9.git branch -D tmp<br>
<br>
10.git push -u origin main<br>
<b>whoaa all your files are commited</b>


<b>CLONE REPO</b>
$ git clone [path-to-repository-to-clone]<br>
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
