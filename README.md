# check_filechange
This Nagios plugin monitors the state of files/directors, using the inotify State Monitoring tool, receiving as arguments the states and files/directors to be monitored, as well as the path of the log file, where the inotify registers the events, notifying the critical state if a state is changed. NB.: Your execution requires installing the inotify-tools.
