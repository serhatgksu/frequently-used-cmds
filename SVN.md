
### Install SVN

     sudo apt-get install subversion
     
### Create SVN
     https://help.ubuntu.com/community/Subversion

### CMD

     svn co svn://122.114.59.116/src/py-rpc
     svn status
     svn update
     svn add timer.py sql.py
     svn commit -m sql-guide
     
### Change User

     svn relocate protocol://currentUser@server/path protocol://newUser@server/path
     svn commit --username newUser
     svn co --username newUser
     svn info
     
