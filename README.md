Start a browser instance in its own namespace.  Requires nsmnt (github:stuscode/nsmnt).


quick start:
start_browser browser_name basedir config_name

Where:
 *browser_name is one of:  firefox, brave, chrome or chromium.
 *basedir is a directory to store configuration directories
 *config_name is the name of the configuration directory for this launch

Default is a special configuration name.  It can be used, but it can also be used as the source configuration to be copied from in case there is no configuration config_name yet.


firefox:
To initialize this method with an existing profile, create a profile directory in the basedir.
Move the existing profile directory into this new profile directory as a subdir.
in the new profile directory create a profile.ini file that looks like:

<pre>
[Profile0]
Name=google
IsRelative=1
Path=ztl4gzoq.google-18576
Default=1

[General]
StartWithLastProfile=1
Version=2
</pre>


'Path' should be the name of the profile subdir, that was the name of the existing profile.  'Name' should be whatever you want to call this profile.
