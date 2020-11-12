# Nirsoft BrowsingHistoryView

This is a distribution of https://www.nirsoft.net/utils/browsing_history_view.html

The original binary is built as a GUI application, and therefore can
not be started by a process running as a service (because there are no
desktops). Additionally it is hard to use in a script because it exits
as soon as the gui is launched (even in CLI mode) so the script can
not wait for it to complete.

This modification sets the console bit in the binary so Windows will
wait for the process to terminate before continuing.
