# Programming Cheatsheet

This repo contains useful tips which are sometimes needed during programming.

# Table of Contents
- [Linux](#linux)
  - [xargs - Using subshell with xargs and docker](#xargs---using-subshell-with-xargs-and-docker)
- [Git](#git)
  - [Tag commit and push it](#tag-commit-and-push-it)
- [Bash](#bash)
  - [Running multiple commands in one line in shell](#running-multiple-commands-in-one-line-in-shell)

## Linux 

### xargs - Using subshell with xargs and docker

> Returned text from first execution will be passed to the second command

```bash
$ docker images artifactory.mrgreen.tech/docker/gametek/sportsbook/sb-mfe:latest -q | xargs docker stop
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
