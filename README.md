Start a browser instance in in its own namespace.  Requires nsmnt (github:stuscode/nsmnt).


quick start:
start_browser browser_name basedir config_name

Where:
browser_name is one of:  firefox, brave, chrome or chromium.
basedir is a directory to keep configuration directories
config_name is the name of the configuration direcotry for this launch

Default is a special configuration name.  It can be used, but it can also be used as the source configuration to be copied from in case there is no configuration config_name yet.


