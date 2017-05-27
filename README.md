# check_filechange
File and/or directorial monitoring. 

Files are groupings of records that follow a structural rule, and may contain data, documents, or programs, stored in a board, which is a mechanism that allows you to organize files according to the subjects they relate to.
Several are the files/directors of the system or not, whose state (open, close, changing, moving, deleting, renaming, or creating is to remain unchanged, and therefore the change in the state of these can be a hint of security problems, and your monitoring is a great solution to ensure that undesirable situations occur in an unnoticed way.

This Nagios plugin monitors the state of files/directors, using the inotify State Monitoring tool, receiving as arguments the states and files/directors to be monitored, as well as the path of the log file, where the inotify registers the events, notifying the critical state if a state is changed.
NB.: Your execution requires installing the inotify-tools.


Mandatory arguments The following arguments must be specified when the module is executed:

-p or --path used to specify the full path of the log file of inotify.

-e or --events used to specify the events to be monitored.

-f or --files used to specify the principals or files to be monitored.

Optional arguments: The following arguments are optionally invoked, as user needs:

-V or --version used to query the module version.

-A or --author used to query the author's data.

Command-Line Execution Example:

./check_filechange -p /var/log/inotify/inotify.log -f /home/cgs/ -e access,open

