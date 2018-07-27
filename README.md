Virtualhost Manage Script
===========

Bash Script to allow create or delete apache virtual hosts on Ubuntu on a quick way.
This script also support SSL, it means HTTPS is available.

## Installation ##

1. Download the script
2. Edit variables in the script (such as target directory for ssl certificates)
3. Apply permission to execute:

```
$ chmod +x /path/to/virtualhost.sh
```

4. Optional: if you want to use the script globally, then you need to copy the file to your /usr/local/bin directory, is better
if you copy it without the .sh extension:

```bash
$ sudo cp /path/to/virtualhost.sh /usr/local/bin/virtualhost
```

### For Global Shortcut ###

```bash
$ cd /usr/local/bin
$ wget -O virtualhost https://raw.githubusercontent.com/RoverWire/virtualhost/master/virtualhost.sh
$ chmod +x virtualhost
```

## Usage ##

Basic command line syntax:

```bash
$ sudo sh /path/to/virtualhost.sh [create | delete | list] [domain] 
```

With script installed on /usr/local/bin

```bash
$ sudo virtualhost [create | delete | list] [domain] 
```

### Examples ###

to create a new virtual host:

```bash
$ sudo virtualhost create mysite.dev
```
to delete a virtual host

```bash
$ sudo virtualhost delete mysite.dev
```
