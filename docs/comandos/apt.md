## adduser

```
adduser

User addition utility.
More information: https://manned.org/adduser.

 - Create a new user with a default home directory and prompt the user to set a password:
   adduser username

 - Create a new user without a home directory:
   adduser --no-create-home username

 - Create a new user with a home directory at the specified path:
   adduser --home path/to/home username

 - Create a new user with the specified shell set as the login shell:
   adduser --shell path/to/shell username

 - Create a new user belonging to the specified group:
   adduser --ingroup group username
 
```

## apt

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

## cd

```
cd

Change the current working directory.
More information: https://manned.org/cd.

 - Go to the specified directory:
   cd path/to/directory

 - Go up to the parent of the current directory:
   cd ..

 - Go to the home directory of the current user:
   cd

 - Go to the home directory of the specified user:
   cd ~username

 - Go to the previously chosen directory:
   cd -

 - Go to the root directory:
   cd /
   
```

## chgrp

```
chgrp

Change group ownership of files and directories.
More information: https://www.gnu.org/software/coreutils/manual/html_node/chgrp-invocation.html.

 - Change the owner group of a file/directory:
   chgrp group path/to/file_or_directory

 - Recursively change the owner group of a directory and its contents:
   chgrp [-R|--recursive] group path/to/directory

 - Change the owner group of a symbolic link:
   chgrp [-h|--no-dereference] group path/to/symlink

 - Change the owner group of a file/directory to match a reference file:
   chgrp --reference path/to/reference_file path/to/file_or_directory
   
```

## chmod

```
chmod

Change the access permissions of a file or directory.
More information: https://www.gnu.org/software/coreutils/manual/html_node/chmod-invocation.html.

 - Give the [u]ser who owns a file the right to e[x]ecute it:
   chmod u+x path/to/file

 - Give the [u]ser rights to [r]ead and [w]rite to a file/directory:
   chmod u+rw path/to/file_or_directory

 - Remove e[x]ecutable rights from the [g]roup:
   chmod g-x path/to/file

 - Give [a]ll users rights to [r]ead and e[x]ecute:
   chmod a+rx path/to/file

 - Give [o]thers (not in the file owner's group) the same rights as the [g]roup:
   chmod o=g path/to/file

 - Remove all rights from [o]thers:
   chmod o= path/to/file

 - Change permissions recursively giving [g]roup and [o]thers the ability to [w]rite:
   chmod [-R|--recursive] g+w,o+w path/to/directory

 - Recursively give [a]ll users [r]ead permissions to files and e[X]ecute permissions to sub-directories within a directory:
   chmod [-R|--recursive] a+rX path/to/directory
   
```

## chown

```
chown

Change user and group ownership of files and directories.
More information: https://www.gnu.org/software/coreutils/manual/html_node/chown-invocation.html.

 - Change the owner user of a file/directory:
   chown user path/to/file_or_directory

 - Change the owner user and group of a file/directory:
   chown user:group path/to/file_or_directory

 - Change the owner user and group to both have the name user:
   chown user: path/to/file_or_directory

 - Recursively change the owner of a directory and its contents:
   chown [-R|--recursive] user path/to/directory

 - Change the owner of a symbolic link:
   chown [-h|--no-dereference] user path/to/symlink

 - Change the owner of a file/directory to match a reference file:
   chown --reference path/to/reference_file path/to/file_or_directory

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

## ls

```
ls

List directory contents.
More information: https://www.gnu.org/software/coreutils/manual/html_node/ls-invocation.html.

 - List files one per line:
   ls -1

 - List all files, including hidden files:
   ls [-a|--all]

 - List files with a trailing symbol to indicate file type (directory/, symbolic_link@, executable*, ...):
   ls [-F|--classify]

 - List all files in [l]ong format (permissions, ownership, size, and modification date):
   ls [-la|-l --all]

 - List files in [l]ong format with size displayed using human-readable units (KiB, MiB, GiB):
   ls [-lh|-l --human-readable]

 - List files in [l]ong format, sorted by [S]ize (descending) recursively:
   ls [-lSR|-lS --recursive]

 - List files in [l]ong format, sorted by [t]ime the file was modified and in reverse order (oldest first):
   ls [-ltr|-lt --reverse]

 - Only list directories:
   ls [-d|--directory] */
   
```

## mkdir

```
mkdir

Create directories and set their permissions.
More information: https://www.gnu.org/software/coreutils/manual/html_node/mkdir-invocation.html.

 - Create specific directories:
   mkdir path/to/directory1 path/to/directory2 ...

 - Create specific directories and their parents if needed:
   mkdir [-p|--parents] path/to/directory1 path/to/directory2 ...

 - Create directories with specific permissions:
   mkdir [-m|--mode] rwxrw-r-- path/to/directory1 path/to/directory2 ...

 - Create multiple nested directories recursively:
   mkdir [-p|--parents] {{path/to/{a,b}/{x,y,z}/{h,i,j}}}
   
```

## rm

```
rm

Remove files or directories.
See also: rmdir.
More information: https://www.gnu.org/software/coreutils/manual/html_node/rm-invocation.html.

 - Remove specific files:
   rm path/to/file1 path/to/file2 ...

 - Remove specific files ignoring nonexistent ones:
   rm [-f|--force] path/to/file1 path/to/file2 ...

 - Remove specific files interactively prompting before each removal:
   rm [-i|--interactive] path/to/file1 path/to/file2 ...

 - Remove specific files printing info about each removal:
   rm [-v|--verbose] path/to/file1 path/to/file2 ...

 - Remove specific files and directories recursively:
   rm [-r|--recursive] path/to/file_or_directory1 path/to/file_or_directory2 ...

 - Remove empty directories (this is considered the safe method):
   rm [-d|--dir] path/to/directory
   
```

## useradd

```
useradd

Create a new user.
See also: users, userdel, usermod.
More information: https://manned.org/useradd.

 - Create a new user:
   sudo useradd username

 - Create a new user with the specified user ID:
   sudo useradd [-u|--uid] id username

 - Create a new user with the specified shell:
   sudo useradd [-s|--shell] path/to/shell username

 - Create a new user belonging to additional groups (mind the lack of whitespace):
   sudo useradd [-G|--groups] group1,group2,... username

 - Create a new user with the default home directory:
   sudo useradd [-m|--create-home] username

 - Create a new user with the home directory filled by template directory files:
   sudo useradd [-k|--skel] path/to/template_directory [-m|--create-home] username

 - Create a new system user without the home directory:
   sudo useradd [-r|--system] username
   
```
