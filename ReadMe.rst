gen-hosts
================================================================================
| This script takes a list of URLs pointing to adblocker filters, hostsfiles, and domain lists.
  It then converts them into hostsfiles, and merges them together.
  The final result is located at `./hosts`.
  It's useful for doing batch operations.
  You could run this script daily, for example, to ensure that your hosts file is always up-to-date.

Dependencies
--------------------------------------------------------------------------------
| A hostsblock (https://github.com/wwalexander/hostsblock)
  binary must be located in the same directory as gen-hosts, if you want to use
  adblocker filters.

Usage
--------------------------------------------------------------------------------
| ``gen-hosts file.list``

Configuration
--------------------------------------------------------------------------------
| gen-hosts requires a textfile containing the URLs to blocklists.
| This textfile should have one entry per line.

- Blank lines are ignored.
- Comments are prefixed by '#'.
- Hostsfiles are prefixed by '@'.
- Domain lists are prefixed by '&'.
- All other lines are assumed to be adblock filters.

Copyright
--------------------------------------------------------------------------------
| gen-hosts is Copyright (C) from 2018 by Miles B Huff per GNU General Public License v3.
