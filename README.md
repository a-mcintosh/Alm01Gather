#BBCP, deb, git

A directory tree with multiple simultaneous uses.

This is a git archive, and also a ready to use filesystem for
  dpkg-deb --build --root-owner-group `readlink -f .`
  
To use git:
    do what you normally would do
    also, git commit -F to-do-prospective-revision.txt
    
To use one or more subsystems in 
  Black Box Component Builder:
  
  cd ./usr/lib/bbcb/.
    none, one, or many subsystems may be here.  Creating a new subsystem, or compiling modules creates content here.
  bbcb
  
Using this approach, a set of subsystems may be added or removed from the installed bbcb directory.

To quickly set up a new archive:
  git clone old new
  git branch --list
  git branch -b <your branch name>
  git branch -d <old branch names>
