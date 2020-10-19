# Programming Cheatsheet

This repo contains useful tips which are sometimes needed during programming.

# Table of Contents
- [Linux](#linux)
  - Folders structure
  - [xargs - Using subshell with xargs and docker](#xargs---using-subshell-with-xargs-and-docker)
  - Update grub 
  - Manage users and privilages
    - Commands
    - Read More
- [Git](#git)
  - [Tag commit and push it](#tag-commit-and-push-it)
- [Bash](#bash)
  - [Running multiple commands in one line in shell](#running-multiple-commands-in-one-line-in-shell)
- [Docker](#docker)
  - Stop all containers
  - Remove all containers

## Linux 

### Folders structure

`/bin` binaries - programs or applications (cat, ls, cp)
`/sbin` system binaries
`/boot` - bootloader, everything what system needs to start running
`/dev` - where devices lives, 
  `/char`
  `/sda` - sda1, sda2
`/etc` - storing configuration (sources.list, cron, application settings)
`/home` - contains users home folders, for personal files and documents
`/lib` - libraries
`/media` - usually systems mount drivers automaticaly here (pendrives, cdroms)
`/mnt` mount - folder to mount manually all drivers (pendrives, cdroms, network drives)
`/opt` optional - folder to manual install software (virtualbox, printer software)
`/proc` - sudo files, for system processes
`/root` - root user home folder
`/run` - tempfs files system, files to faster start system
`/snap`
`/srv` - service directory (ftp server, http server)
`/sys` system - similar to `/run` directory, installed during the boot start system
`/tmp` temporary - temporary director for programs during session, you can recover something from there
`/usr` user - user applications
 `/local`
 `/src`
 `/share`
`/var` - variable directory
  `/crash`
  `/logs` for system and any diffrent applications
 
### xargs - Using subshell with xargs and docker

> Returned text from first execution will be passed to the second command

```bash
$ docker images artifactory.mrgreen.tech/docker/gametek/sportsbook/sb-mfe:latest -q | xargs docker stop
```

### Usefull commands

```bash
$ updatedb 
$ locate [file]
$ passwd
$ man [command]
$ [command] --help
```

### Update grub 

```bash
$ sudo update-grub
```

### Manage users and privilages

```bash
-rw-r--r--@  1 kubek  staff  20484 Oct 18 15:28 some_file.txt
drwxr-xr-x  19 kubek  staff    608 Oct 18 15:28 some_folder
```

First letter says about `-` file or `d` folder (directory). Next are tell us about access to this specific file/folder. 

| # |        Permission       | rwx | Binary |
|:-:|:-----------------------:|:---:|:------:|
| 7 | read, write and execute | rwx | 111    |
| 6 | read and write          | rw- | 110    |
| 5 | read and execute        | r-x | 101    |
| 4 | read only               | r-- | 100    |
| 3 | write and execute       | -wx | 011    |
| 2 | write only              | -w- | 010    |
| 1 | execute only            | --x | 001    |
| 0 | none                    | --- | 000    |

You can modify access using command `chmod`, fe.

```bash
$ chmod 0664 sharedFile
```

#### Commands

```bash
$ adduser [user name] #add new user to the system
$ cat /etc/passwd #show users
$ cat /etc/shadow #show users and passwords
$ su [user-name] #switch to provided user
```

#### Read more

[Shadow Passwords](https://www.cyberciti.biz/faq/understanding-etcshadow-file)
[Crack users passwords](https://null-byte.wonderhowto.com/how-to/crack-shadow-hashes-after-getting-root-linux-system-0186386/)

### Manage networks

```bash
$ ifconfig #shows you network interfaces available for you
$ iwconfig #shows you only wireless adapters
$ ping [server-ip-address]
$ arp -a
$ netstat -ano #shows you connections which are running on you machine
$ router #shows you routing table - where you traffic is exit essentially 
```

### Manage files (create|modify|remove)

```bash
$ nano new-file.txt
$ touch new-file.txt
$ gedit new-file.txt
$ echo "tekst" > new-file.txt #create file and override with text
$ echo "tekst" >> new-file.txt #create file and save text at the bottom of file 
```

### Manage services (start|stop)

```bash
$ service apache2 start #start apache server
$ python -m SimpleHTTPServer 80 #run python server which is smiler than apatche and can be run in every folder
$ systemctl enable postgresq #run for example postgres database not only fot that session but also after reboot machine
```

## Git

### Tag commit and push it

example:
```bash
$ git tag v1.7.7-beta.20 d43bab9
$ git push origin master --tags
```

## Bash 

### Running multiple commands in one line in shell

- `|` pipes (pipelines) the standard output (stdout) of one command into the standard input of another one. Note that stderr still goes into its default destination, whatever that happen to be.
- `|&` pipes both stdout and stderr of one command into the standard input of another one. Very useful, available in bash version 4 and above.
- `&&` executes the right-hand command of && only if the previous one succeeded.
- `||` executes the right-hand command of || only it the previous one failed.
- `;` executes the right-hand command of ; always regardless whether the previous command succeeded or failed. Unless set -e was previously invoked, which causes bash to fail on an error.

[stackoverflow question](https://stackoverflow.com/questions/5130847/running-multiple-commands-in-one-line-in-shell)

## Docker

### Stop all containers

```bash
docker kill $(docker ps -q)
```

### Remove all containers

```bash
docker rm $(docker ps -a -q)
```
