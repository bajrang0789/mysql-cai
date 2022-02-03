# mysql-cai
MySQL Check Auto-Increment

# Purpose

This tool can be used as a Nagios monitoring plugin.

It checks if mysql `AUTOINCREMENT` columns are getting close to overflow.

By default it produces a `WARNING` if any autoincrement value reaches
70% of the maximal value that can be stored in the column, and a
`CRITICAL` if it reaches more than 85% of the maximal value.

# Options

Please run

    perldoc -F check.autoincrement

to read the tool's documentation, including the options.

# Issues

Incase you get the below error: 
`You need to install the perl-doc package to use this program.`
you might need to install the perl-doc package.
On ubuntu: 
`apt-get install perl-doc`
