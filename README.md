#BBCP, deb, git

A directory structure with multiple simultaneous uses.

This is a .deb staging area.
  dpkg-deb --build --root-owner-group `readlink -f .`
  
This is a git archive.
    Do what you normally do using git.
    
      gedit to-do-prospective-revision.txt
      git commit -F to-do-prospective-revision.txt


This is a user directory in BBCB.
    Do what you normally do in BBCP.
  
      cd ./usr/lib/bbcb/.
      bbcb &
  
Multiple subsystems are stored in multiple git branches
  git branch --list
  git checkout create-sandbox
  git branch -b <your new subsystem>

Recommended use is to git commit, create a .deb, and install a subsystem, then work on the other subsystem.

