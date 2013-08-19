Xide - remote code editor
=========================

This project came about due to the problem I had working on an old version of OSX and couldnt install a decent editor (sublime). At the same time I was doing a lot of work on my EC2 servers. I wanted to be able to just write/edit the project in place because I was prototyping some stuff, and I began writing Xide so that I can spin up an editor for any project.

How it works
------------

Xide is a command line tool (Hopefully when it is complete enough it will be on NPM for easier install) which allows you to spin up hosted web-based IDE's (code editors) on remote servers, and allows you to edit your projects code in a specified directory (and not above it).


Commands
--------

      xide start /home/my_user/my_proj/ 9090
      
The "xide start [root_dir] [port]" command starts a new editor. It requires two arguments: root directory and port to host the editor at. 
      
      xide list 
      
The "xide list" command lists all the editors which are currently running, as well as their root directories and ports they are running on.
      
      xide stop 9090
      
The "xide stop [port]" command will stop/remove the editor currently running on the specified port, which is it's only argument.


License
-------

MIT license. If you are not familiar with MIT style licenses please refer to the "LICENSE" file.
(c) Timothy Cubbedge (github.com/timcubb) 
www.TimothyCubbedge.com
www.zenoku.com

