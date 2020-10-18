# Programming Cheatsheet

This repo contains useful tips which are sometimes needed during programming.

# Table of Contents
- [Linux](#linux)
  - [xargs - Using subshell with xargs and docker](#xargs---using-subshell-with-xargs-and-docker)
- [Git](#git)
  - [Tag commit and push it](#tag-commit-and-push-it)
- [Bash](#bash)
  - [Running multiple commands in one line in shell](#running-multiple-commands-in-one-line-in-shell)
- [Docker](#docker)
  - Stop all containers
  - Remove all containers

## Linux 

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

### Users and privilages

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

### Update grub 

```bash
$ sudo update-grub
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
