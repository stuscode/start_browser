Start a browser instance in its own namespace.  Requires nsmnt (github:stuscode/nsmnt).


quick start:
start_browser browser_name basedir config_name

Where:
browser_name is one of:  firefox, brave, chrome or chromium.
basedir is a directory to store configuration directories
config_name is the name of the configuration directory for this launch

Default is a special configuration name.  It can be used, but it can also be used as the source configuration to be copied from in case there is no configuration config_name yet.


firefox:
If there is an existing profile, create a profile directory in the basedir.
Move the profile directory into this new profile directory as a subdir.
in the new profile directory create a profile.ini file that looks like:

[Profile0]<br>
Name=google<br>
IsRelative=1<br>
Path=ztl4gzoq.google-18576<br>
Default=1<br>
<br>
[General]<br>
StartWithLastProfile=1<br>
Version=2<br>


Path should be the name of the profile subdir.  The Name should be whatever you
want to call this profile.
