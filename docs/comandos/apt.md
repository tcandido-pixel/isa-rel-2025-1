# apt

```
apt 2.6.1 (amd64)
Usage: apt [options] command

apt is a commandline package manager and provides commands for
searching and managing as well as querying information about packages.
It provides the same functionality as the specialized APT tools,
like apt-get and apt-cache, but enables options more suitable for
interactive use by default.

Most used commands:
  list - list packages based on package names
  search - search in package descriptions
  show - show package details
  install - install packages
  reinstall - reinstall packages
  remove - remove packages
  autoremove - automatically remove all unused packages
  update - update list of available packages
  upgrade - upgrade the system by installing/upgrading packages
  full-upgrade - upgrade the system by removing/installing/upgrading packages
  edit-sources - edit the source information file
  satisfy - satisfy dependency strings

See apt(8) for more information about the available commands.
Configuration options and syntax is detailed in apt.conf(5).
Information about how to configure sources can be found in sources.list(5).
Package and version choices can be expressed via apt_preferences(5).
Security details are available in apt-secure(8).
                                   Este APT tem Poderes de Super Vaca.
```
## tldr

```
apt

Package manager for Debian-based distributions.
Intended as a user-friendly alternative to apt-get for interactive use.
For equivalent commands in other package managers, see https://wiki.archlinux.org/title/Pacman/Rosetta.
More information: https://manned.org/apt.8.

 - Update the list of available packages and versions (recommended before running other apt commands):
   sudo apt update

 - Search packages by name or description:
   apt search package

 - Search packages by name only (supports wildcards like *):
   apt list package

 - Show detailed information about a package:
   apt show package

 - Install a package, or update it to the latest version:
   sudo apt install package

 - Remove a package (use purge instead to also remove configuration files):
   sudo apt remove package

 - Upgrade all installed packages to their latest versions:
   sudo apt upgrade

 - List all installed packages:
   apt list [-i|--installed]

```
## cp

```
cp

Copy files and directories.
More information: https://www.gnu.org/software/coreutils/manual/html_node/cp-invocation.html.

 - Copy a file to another location:
   cp path/to/source_file.ext path/to/target_file.ext

 - Copy a file into another directory, keeping the filename:
   cp path/to/source_file.ext path/to/target_parent_directory

 - Recursively copy a directory's contents to another location (if the destination exists, the directory i>
   cp [-r|--recursive] path/to/source_directory path/to/target_directory

 - Copy a directory recursively, in verbose mode (shows files as they are copied):
   cp [-vr|--verbose --recursive] path/to/source_directory path/to/target_directory

 - Copy multiple files at once to a directory:
   cp [-t|--target-directory] path/to/destination_directory path/to/file1 path/to/file2 ...

 - Copy all files with a specific extension to another location, in interactive mode (prompts user before >
   cp [-i|--interactive] *.ext path/to/target_directory

 - Follow symbolic links before copying:
   cp [-L|--dereference] link path/to/target_directory

 - Use the full path of source files, creating any missing intermediate directories when copying:
   cp --parents source/path/to/file path/to/target_file

```

