| Operation / command name | What it does | What I observed |
| :--- | :--- | :--- |
| Current-directory display | Displays current working directory | /Users/ejazahamedkhan/Documents/digital_detective |
| Directory listing | Displays directories | directory names |
| Detailed listing | Displays amount & directories | amount of directories |
| Change directory | changes directory | changed directory |
| Create directory | creates directory | creates directory |
| Create empty file | creates empty file | creates empty file |
| Copy file | copy file | copied file |
| Move / rename file | moves file | file moved |
| Display file contents | displays file contents | file contents |
```[cite: 2]

1. we use echo > to replace the file contents and echo >> to add text to the end without replacing any file content
2. copying a file doesnt change original file but moving it deletes old and creates new replica at destination
3. current working directory provides the address for the user to understand which working directory they are working in.
4. directory listing operation is useful as we can analyze all the chmods of all directories along with their names

# normal directory listing
ejazahamedkhan@192 digitaldetective % ls -l
total 8
drwxr-xr-x  2 ejazahamedkhan  staff  64 12 Nov 12:44 evidence
drwxr-xr-x  3 ejazahamedkhan  staff  96 12 Nov 12:42 mission-00-setup
drwxr-xr-x  3 ejazahamedkhan  staff  96 12 Nov 12:42 mission-01-computer-basics
drwxr-xr-x  3 ejazahamedkhan  staff  96 12 Nov 12:42 mission-02-terminal
drwxr-xr-x  3 ejazahamedkhan  staff  96 12 Nov 12:42 mission-03-operating-systems
drwxr-xr-x  3 ejazahamedkhan  staff  96 12 Nov 12:42 mission-04-programs
drwxr-xr-x  3 ejazahamedkhan  staff  96 12 Nov 12:43 mission-05-numbers-data
drwxr-xr-x  3 ejazahamedkhan  staff  96 12 Nov 12:43 mission-06-git-github
drwxr-xr-x  3 ejazahamedkhan  staff  96 12 Nov 12:43 mission-07-networking
drwxr-xr-x  3 ejazahamedkhan  staff  96 12 Nov 12:43 mission-08-final-report
-rw-r--r--  1 ejazahamedkhan  staff  24 12 Nov 12:43 README.md
ejazahamedkhan@192 digitaldetective %

# detailed directory listing
ejazahamedkhan@192 digitaldetective % ls -la
total 8
drwxr-xr-x  14 ejazahamedkhan  staff   448 12 Nov 12:46 .
drwx------@ 37 ejazahamedkhan  staff  1184 12 Nov 12:46 ..
drwxr-xr-x  13 ejazahamedkhan  staff   416 12 Nov 12:46 .git
drwxr-xr-x   2 ejazahamedkhan  staff    64 12 Nov 12:44 evidence
drwxr-xr-x   3 ejazahamedkhan  staff    96 12 Nov 12:42 mission-00-setup
drwxr-xr-x   3 ejazahamedkhan  staff    96 12 Nov 12:42 mission-01-computer-basics
drwxr-xr-x   3 ejazahamedkhan  staff    96 12 Nov 12:42 mission-02-terminal
drwxr-xr-x   3 ejazahamedkhan  staff    96 12 Nov 12:42 mission-03-operating-systems
drwxr-xr-x   3 ejazahamedkhan  staff    96 12 Nov 12:42 mission-04-programs
drwxr-xr-x   3 ejazahamedkhan  staff    96 12 Nov 12:43 mission-05-numbers-data
drwxr-xr-x   3 ejazahamedkhan  staff    96 12 Nov 12:43 mission-06-git-github
drwxr-xr-x   3 ejazahamedkhan  staff    96 12 Nov 12:43 mission-07-networking
drwxr-xr-x   3 ejazahamedkhan  staff    96 12 Nov 12:43 mission-08-final-report
-rw-r--r--   1 ejazahamedkhan  staff    24 12 Nov 12:43 README.md

A pipe symbol is used to send the ouput of the command to the rhs of the pipe for processing.
