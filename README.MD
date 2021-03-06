# adminpy - Python Admin access for most platforms

This module makes it easy to check system platform type and gain admin rights for scripts that require it.

This utilises PyUAC on the Windows platform and requires the use of Sudo on *NIX systems for admin rights escalation.

The purpose of this is to try and make people's life easier when needed more rights for python scripts.

[adminpy on PyPI](https://pypi.org/project/adminpy)

# Usage of the module

There are 3 functions of this module

1. The sysinfo() function outputs whether the script recognises which type of system it's running on.

Example: On a Windows system, the script will output,"You are running on a Windows-based system."

2. The admincheck() function will output a "Yes" or "No", depending on if it has root or admin privilege

3. The runadmin() function will utilise ctypes function or Sudo (for linux) to relaunch script if does not have root or admin privilege

# Requirements

* This module requires [PyUAC](https://github.com/Preston-Landers/pyuac) and [PyWin32](https://pypi.org/project/pywin32/) package to be installed on a Windows system.
* This module requires Python 3, and does not support Python 2.

# License
See the [LICENSE file](LICENSE).