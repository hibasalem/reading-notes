## Git

Version Control is a system that allows us to revisit various versions of files we can revert files to a previous version by (VCS), Local VCS entails one database on your hard disk that stores changes to files but there is also a Centralized Version Control System (CVCS)(storing server), the CVCS considered as a single point of failure so there is Distributed Version Control systems (DVCS)
Git is a DVCS that stores data in a file system by snapshots, it relies on local operations and every single change applied to any file or directory is tracked by Git, Files in Git can reside in three main states: committed(securely stored in a local database), modified(changed but not committed to the database) and staged.

The local Git repository has three components:
Working Directory: The actual files reside here, Index: The area used for staging, Head: Points to the most recent commit
files in a check out are either in a tracked (can be modified, unmodified, or staged; they were part of the most recent file snapshot) or untracked state(were not in the last snapshot and do not currently reside in the staging area)

The life cycle of file status 
![The life cycle of file status](https://blog.udemy.com/wp-content/uploads/2015/08/image006.png)