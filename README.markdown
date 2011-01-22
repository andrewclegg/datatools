datatools
=========

Command line tools for data analysis.

Similar (and complementary) to bitly's data_hacks: https://github.com/bitly/data_hacks/

Installing: Just copy the scripts to somewhere in your path. I'll add a setup script later when there's enough in here to warrant a proper release. Run scripts with -h option for usage.

Tested with Python 2.6.6 on Ubuntu 10.10, should work anywhere, no external dependencies.

date_select
-----------

Select date range from timestamped, chronologically-ordered files (or stdin) such as logfiles.

Example:

    $ date_select -s 21/Jan/2011:17:00:00 -e 22/Jan/2011:17:00:00 access.log.1 access.log

You can supply an alternate timestamp format (in strptime notation), and a regex for locating the timestamp in each line, if the defaults don't work.

