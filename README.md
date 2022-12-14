# Programming Cheatsheet

This repo contains useful tips which are sometimes needed during programming.

## Table of Contents

<details>
<summary><b>Expand Table</b></summary>

- [Programming Cheatsheet](#programming-cheatsheet)
  - [Table of Contents](#table-of-contents)
  - [General](#general)
    - [Google search queries](#google-search-queries)
  - [General Computer Problems](#general-computer-problems)
    - [Convert movies to another format](#convert-movies-to-another-format)
  - [Browsers](#browsers)
    - [Can I modify javascript bundle in firefox?](#can-i-modify-javascript-bundle-in-firefox)
  - [General Programmimng](#general-programmimng)
    - [Example of `README.md` file](#example-of-readmemd-file)
    - [Example of `CHANGELOG.md`](#example-of-changelogmd)
    - [What are the different kinds of cases](#what-are-the-different-kinds-of-cases)
  - [Mac OS](#mac-os)
    - [Zip file/folder with password](#zip-filefolder-with-password)
    - [Show/hide hidden files](#showhide-hidden-files)
    - [Delete all .DS_Store files](#delete-all-ds_store-files)
    - [Find and kill process](#find-and-kill-process)
  - [AWS](#aws)
    - [Serverless Framework vs AWS Serverless Application Model (SAM)](#serverless-framework-vs-aws-serverless-application-model-sam)
  - [Firebase](#firebase)
    - [CLI Commands](#cli-commands)
    - [Run local functions using different port](#run-local-functions-using-different-port)
  - [Linux](#linux)
    - [Linux Commands](#linux-commands)
    - [How to check current user](#how-to-check-current-user)
    - [Check current shell path](#check-current-shell-path)
    - [Change the shell path from/to bash/zsh](#change-the-shell-path-fromto-bashzsh)
    - [Check the linux distribution](#check-the-linux-distribution)
    - [How to merge two or more mp3 files](#how-to-merge-two-or-more-mp3-files)
    - [Envs](#envs)
    - [Folders structure](#folders-structure)
    - [xargs - Using subshell with xargs and docker](#xargs---using-subshell-with-xargs-and-docker)
    - [Usefull commands](#usefull-commands)
    - [Update grub](#update-grub)
    - [Manage users and privilages](#manage-users-and-privilages)
    - [Zip/Unzip files](#zipunzip-files)
      - [Commands](#commands)
      - [Read more](#read-more)
    - [Manage networks](#manage-networks)
    - [Manage files (create|modify|remove)](#manage-files-createmodifyremove)
    - [Manage services (start|stop)](#manage-services-startstop)
    - [How to find files matched to pattern](#how-to-find-files-matched-to-pattern)
    - [How to remove found files](#how-to-remove-found-files)
    - [How to save command results in file](#how-to-save-command-results-in-file)
  - [Javascript](#javascript)
    - [How initialize eslint in project with predefined configuration](#how-initialize-eslint-in-project-with-predefined-configuration)
  - [Node.js](#nodejs)
    - [How to create executable node.js file](#how-to-create-executable-nodejs-file)
    - [How to read file content?](#how-to-read-file-content)
    - [Default prettier configuration](#default-prettier-configuration)
  - [npm](#npm)
    - [Package.json configuration](#packagejson-configuration)
    - [Informations about npm package](#informations-about-npm-package)
    - [How to use local npm package in another project](#how-to-use-local-npm-package-in-another-project)
    - [What is scope and how to use it](#what-is-scope-and-how-to-use-it)
    - [Private repository](#private-repository)
    - [How to versionize packages](#how-to-versionize-packages)
    - [How to use versions in `package.json`](#how-to-use-versions-in-packagejson)
    - [You can set up version of package](#you-can-set-up-version-of-package)
    - [Packages installation flags for `npm install` command](#packages-installation-flags-for-npm-install-command)
    - [Show installed npm packages](#show-installed-npm-packages)
    - [Print the folder where npm will install executables](#print-the-folder-where-npm-will-install-executables)
    - [Try to run package from the nearest (or local project) executor](#try-to-run-package-from-the-nearest-or-local-project-executor)
    - [Link developement package to the project](#link-developement-package-to-the-project)
    - [How to configure eslint?](#how-to-configure-eslint)
    - [How to run a code after npm package installation?](#how-to-run-a-code-after-npm-package-installation)
    - [How to set up registry url and/or @scoped registry link](#how-to-set-up-registry-url-andor-scoped-registry-link)
    - [How to set up files which should be included in npm package](#how-to-set-up-files-which-should-be-included-in-npm-package)
  - [Git](#git)
    - [Popular commands](#popular-commands)
    - [Overwrite master with empty project](#overwrite-master-with-empty-project)
    - [Tag commit and push it](#tag-commit-and-push-it)
    - [How to check number of commits by person](#how-to-check-number-of-commits-by-person)
    - [How to change https to ssh authorization in existing repo](#how-to-change-https-to-ssh-authorization-in-existing-repo)
    - [Show linked remote repository](#show-linked-remote-repository)
    - [Change linked remote repository](#change-linked-remote-repository)
    - [How to revert specific Merge](#how-to-revert-specific-merge)
  - [Bash](#bash)
    - [ZSH and oh-my-zsh - Make bash more intuitive and usefull](#zsh-and-oh-my-zsh---make-bash-more-intuitive-and-usefull)
    - [Add auto suggestions and shell syntax highlight](#add-auto-suggestions-and-shell-syntax-highlight)
    - [Running multiple commands in one line in shell](#running-multiple-commands-in-one-line-in-shell)
  - [Docker](#docker)
    - [Stop all containers](#stop-all-containers)
    - [Remove all containers](#remove-all-containers)

</details>

## General

### Google search queries

- `"what is javascript"` - Exact Match - Use quotes to force an exact-match search:
- `html AND css` - AND operator - AND operator will return only results related to both terms:
- `(javascript OR python) free course` - OR opeator - You can use the OR operator to get the results related - to one of the search terms
- `javascript -css` - Minus operator - operator will exclude results that contain a term or phrase:
- `"how to start * in 6 months"` - Wildcard operator - You can use the (*) wildcards as placeholders, which will be replaced by any word or phrase.
- `site:freecodecamp.org` - Site operator - earch inside a single website.
- `filetype:pdf learn css` - Search by filetype - You can also use a very useful feature that helps to find a specific file type.
- `ecmascript 2016..2018` - Search for a range of numbers.
- `JavaScript|HTML|CSS filetype:pdf -"framework" site:edu` - Google search result for JavaScript PDF documents, limit search to a domain e.g .com, .edu, .org e.t.c

Tips:

You can use | in place of OR. e.g JavaScript | HTML

The ext is also a substitute for filetype

## General Computer Problems

### Convert movies to another format

```sh
brew install ffmpeg
```

Stream copy (-c copy) is like a "copy and paste" so the quality is preserved and the process is fast.

```sh
ffmpeg -i input.mov -c copy output.mp4
ffmpeg -i input.mov -vcodec h264 output.mp4 #copy and modify codec for better compression
```

This will convert the MOV to H.264 video and AAC audio:

```sh
ffmpeg -i input.mov -c:v libx264 -c:a aac -vf format=yuv420p -movflags +faststart output.mp4
```

[ffmpeg homebrew](https://formulae.brew.sh/formula/ffmpeg)
[ffmpeg docs](https://ffmpeg.org/)

## Browsers

### Can I modify javascript bundle in firefox?

You can do it in several ways:

1. You should use javascript console to redefine functions.
2. You can also use fiddler and intercept the code.
3. You can use Firebug console, but is deprecated.
4. You can use [WebReplay Firefox](https://developer.mozilla.org/en-US/docs/Mozilla/Projects/WebReplay), but is deprecated.

> Use `chrome` browser where modified files can be persisted storage.

## General Programmimng

### Example of `README.md` file

[GO TO Readme file](/README-example.md)

### Example of `CHANGELOG.md`

[GO TO Changelog file](/CHANGELOG-example.md)

### What are the different kinds of cases

- `Pascal Case` (Used for Class) => `MyVariable`
- `Camel Case` (Used for variable at Java, C#, etc.) => `myVariable`
- `Flat Case` (Used for package at Java, etc.) => `myvariable`
- `Snake Case` (Used for variable at Python, PHP, etc.) => `my_variable`
- `Kebab Case` (Used for css) => `my-variable`

## Mac OS

### Zip file/folder with password

```sh
zip -er example.zip ./example-folder/*
```

### Show/hide hidden files

```sh
defaults write com.apple.finder AppleShowAllFiles YES; //or NO
killall Finder
```

> You can also use keyboard shortcut `Shift + Command + .`

### Delete all .DS_Store files

```sh
sudo find / -name .DS_Store -delete; killall Finder
```

### Find and kill process

```bash
sudo lsof -i :3000
kill -9 <PID> # kill -15 gives the process a chance to clean up after itself
```

## AWS

### Serverless Framework vs AWS Serverless Application Model (SAM)

SAM on the other hand is an abstraction layer specifically for AWS using not only FaaS but also DynamoDB for storage and API Gateway for creating a serverless HTTP endpoint.

The biggest difference is that Serverless is written to deploy FaaS (Function as a Service) functions to different providers.

https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/sam-cli-command-reference-sam-local-start-lambda.html
https://stackoverflow.com/questions/52228361/whats-the-difference-between-aws-sam-serverless-application-model-and-serverl

## Firebase

[Sapmles of functions](https://github.com/firebase/functions-samples)

### CLI Commands

[CLI Documentation](https://firebase.google.com/docs/cli)

### Run local functions using different port

```bash
firebase serve --only functions --port=9000
```

## Linux

### Linux Commands

[GO TO](/linux-commands.md) Linux Commands

### How to check current user

```sh
# login name
whoami
echo $USER
# or full information
id
# or user name
id -F
# rest of user checkers
id -u  # returns UID
id -un # returns username
id -g  # returns primary (a.k.a. effictive) GID
id -gn # returns primary Group Name
# or currently logged users to system
w
```

### Check current shell path

```sh
echo $0
# or
echo $SHELL
```

### Change the shell path from/to bash/zsh

```sh
chsh -s $(which bash)
chsh -s $(which zsh)
# or specific folder as shell
chsh -s /bin/zsh
```

### Check the linux distribution

```sh
cat /etc/os-release
# or
cat /proc/version

```

### How to merge two or more mp3 files

```sh
cat file1.mp3 > newfile.mp3
cat file1.mp3 file2.mp3 file3.mp3 > newfile.mp3
```

> Only if MP3 files are recorded at the same bitrate.

### Envs

echo $SHELL
echo #ZSH

### Folders structure

- `/bin` binaries - programs or applications (cat, ls, cp)
- `/sbin` system binaries
- `/boot` - bootloader, everything what system needs to start running
- `/dev` - where devices lives,
  - `/char`
  - `/sda` - sda1, sda2
- `/etc` - storing configuration (sources.list, cron, application settings)
- `/home` - contains users home folders, for personal files and documents
- `/lib` - libraries
- `/media` - usually systems mount drivers automaticaly here (pendrives, cdroms)
- `/mnt` mount - folder to mount manually all drivers (pendrives, cdroms, network drives)
- `/opt` optional - folder to manual install software (virtualbox, printer software)
- `/proc` - sudo files, for system processes
- `/root` - root user home folder
- `/run` - tempfs files system, files to faster start system
- `/snap`
- `/srv` - service directory (ftp server, http server)
- `/sys` system - similar to `/run` directory, installed during the boot start system
- `/tmp` temporary - temporary director for programs during session, you can recover something from there
- `/usr` user - user applications
  - `/local`
  - `/src`
  - `/share`
- `/var` - variable directory
  - `/crash`
  - `/logs` for system and any diffrent applications

### xargs - Using subshell with xargs and docker

> Returned text from first execution will be passed to the second command

```bash
docker images artifactory.mrgreen.tech/docker/gametek/sportsbook/sb-mfe:latest -q | xargs docker stop
```

### Usefull commands

```bash
updatedb
locate [file]
passwd
man [command]
[command] --help
```

### Update grub

```bash
sudo update-grub
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
chmod 0664 sharedFile
```

### Zip/Unzip files

```bash
zip -r filename.zip /home/folder/*
unzip html.zip ./
mv ./html/* /home/dazdyqephu/domains/ohsospecial.nl/public_html/
```

#### Commands

```bash
adduser [user name] #add new user to the system
cat /etc/passwd #show users
cat /etc/shadow #show users and passwords
su [user-name] #switch to provided user
```

#### Read more

[Shadow Passwords](https://www.cyberciti.biz/faq/understanding-etcshadow-file)
[Crack users passwords](https://null-byte.wonderhowto.com/how-to/crack-shadow-hashes-after-getting-root-linux-system-0186386/)

### Manage networks

```bash
ifconfig #shows you network interfaces available for you
iwconfig #shows you only wireless adapters
ping [server-ip-address]
arp -a
netstat -ano #shows you connections which are running on you machine
router #shows you routing table - where you traffic is exit essentially
```

### Manage files (create|modify|remove)

```bash
nano new-file.txt
touch new-file.txt
gedit new-file.txt
echo "tekst" > new-file.txt #create file and override with text
echo "tekst" >> new-file.txt #create file and save text at the bottom of file
```

### Manage services (start|stop)

```bash
service apache2 start #start apache server
python -m SimpleHTTPServer 80 #run python server which is smiler than apatche and can be run in every folder
systemctl enable postgresq #run for example postgres database not only fot that session but also after reboot machine
```

### How to find files matched to pattern

```sh
find . -name "*edit*"
```

### How to remove found files

```sh
find . -name "*edit*" -delete
# OR
find . -name "*edit*" -exec rm -rf {} \;
```

### How to save command results in file

```sh
find . -name "*edit*" >> filename.txt
```

## Javascript

### How initialize eslint in project with predefined configuration

```sh
npm install eslint -g
eslint --init

# or

npm install eslit --save-dev
./node_modules/.bin/eslint --init
```

## Node.js

### How to create executable node.js file

Add to the top of file:

```js
#!/usr/bin/env node
```

### How to read file content?

```js
const fs = require('fs-extra');

const fileContent = await fs.readFile('../usage-instruction.txt', 'utf8');
```

### Default prettier configuration

```json
{
    "printWidth": 120,
    "trailingComma": "none",
    "tabWidth": 4,
    "semi": true,
    "singleQuote": true,
    "arrowParens": "avoid"
}
```

## npm

### Package.json configuration

> https://docs.npmjs.com/cli/v7/configuring-npm/package-json#main

### Informations about npm package

```sh
npm info package-name
```

### How to use local npm package in another project

For tests purposes you can add package to `package.json` from your local project folder:

```json
{
  "global-functions": "file:../global-functions",
}
```

### What is scope and how to use it

A scope allows you to create a package with the same name as a package created by another user or organization without conflict. The scope name is everything between the @ and the slash.

- Unscoped packages are always public.

You can setup different repository for specific scope using your `.npmrc` file:

```sh
@myscope:registry=https://mycustomregistry.example.org
```

or use command line for it: `npm config set @myco:registry http://reg.example.com`

### Private repository

Modify `.npmrc` file:

```js
registry=http://npm.differentpage.com/
```

### How to versionize packages

| Code status |        Stage       | Rule | Example version |
|:-:|:-----------------------:|:---:|:------:|
| First release | New product | Start with 1.0.0 | 1.0.0    |
| Backward compatible bug fixes | Patch release | Increment the third digit | 1.0.1 |
| Backward compatible new features | Minor release | Increment the middle digit and reset last digit to zero | 1.1.0    |
| Changes that break backward compatibility | Major release | Increment the first digit and reset middle and last digits to zero | 2.0.0 |

### How to use versions in `package.json`

- Patch releases: 1.0 or 1.0.x or ~1.0.4
- Minor releases: 1 or 1.x or ^1.0.4
- Major releases: * or x

### You can set up version of package

You can setup version of the package directly from npm repository.

Examples:

```sh
# npm version [<newversion> | major | minor | patch | premajor | preminor | prepatch | prerelease [--preid=<prerelease-id>] | from-git]
npm version patch
npm version minor
npm version major
# and combinations with preword "pre"
npm version prepatch
npm version preminor
npm version premajor
# or alfa or beta tags
npm version preminor --preid alfa
npm version prerelease --preid=beta
```

after that you should deploy npm package into the repository:

```sh
npm publish
```

### Packages installation flags for `npm install` command

`common options: [
    -P|--save-prod|
    -D|--save-dev|
    -O|--save-optional
    -E|--save-exact
    -B|--save-bundle
    --no-save
    --dry-run
]`

### Show installed npm packages

You probably have some packages installed globally already on your system. You can see them by typing:

```bash
npm list --depth 0 #for local project

npm list -g --depth 0 #for global npm

# or

ls `npm root -g`
```

### Print the folder where npm will install executables

```sh
npm bin
```

### Try to run package from the nearest (or local project) executor

```sh
$(npm bin)/package_name
```

[run-locally-installed-npm-packages-without-global-install](https://www.rockyourcode.com/run-locally-installed-npm-packages-without-global-install/)

### Link developement package to the project

Copy package from developement npm package into final project:

```bash
npm link #run in npm package
npm link @scope/package-name #run in project
```

After developement process unlink package using:

```sh
npm unlink --no-save @scope/package-name #clear linked packages in project
npm unlink #clear npm links
```

> You can always check if package in linked correctly looking into node_modules.

### How to configure eslint?

The easiest way to install eslint configuration is run command:

```sh
./node_modules/.bin/eslint --init
```

### How to run a code after npm package installation?

You can set up command postinstall in `scripts` property inside of package.json file:

```json
{
  "scripts": {
      "postinstall": "node bin/index.js"
  }
}
```

> https://docs.npmjs.com/cli/v7/using-npm/scripts#npm-ci

### How to set up registry url and/or @scoped registry link

```sh
npm config set registry https://registry.npmjs.org
npm config get @company_name:registry
npm config set @company_name:registry https://artifactory.company.page/artifactory/api/npm/npm/
npm install -g @company_name/package-name
```

### How to set up files which should be included in npm package

The optional files field is an array of file patterns that describes the entries to be included when your package is installed as a dependency. File patterns follow a similar syntax to .gitignore, but reversed: including a file, directory, or glob pattern (*, **/*, and such) will make it so that file is included in the tarball when it's packed. Omitting the field will make it default to ["*"], which means it will include all files.

Some special files and directories are also included or excluded regardless of whether they exist in the files array (see below).

You can also provide a .npmignore file in the root of your package or in subdirectories, which will keep files from being included. At the root of your package it will not override the "files" field, but in subdirectories it will. The .npmignore file works just like a .gitignore. If there is a .gitignore file, and .npmignore is missing, .gitignore's contents will be used instead.

> https://docs.npmjs.com/cli/v7/configuring-npm/package-json#files

## Git

### Popular commands

```sh
git branch  -a #show all branches
            -D #remove branch force

git branch <branch_name> #create new branch

git push origin -d <remote_branch> #remove remote branch

git checkout <branch_name> #swich branch
git checkout -b <branch_name> #create branch and switch

git checkout -b test origin/<remote_branch>
git checkout -t origin/<remote_branch>

git checkout --orphan empty-branch #create empty branch without any history data

git reset --soft origin/<branch> #reset unpushed commits
git reset --hard origin/<branch>

git reset --soft HEAD~1 #reset one commit back
git reset --hard HEAD~1

git fetch <remote_branch> #Update your branch when the original branch from official repository has been updated

git rm -rf . #remove all stashed files

git commit --allow-empty -m "commit_message" #commit empty

git push origin <branch>:<remote_branch> #overwrite remote branch with local
```

[Commands docs](https://www.atlassian.com/git/tutorials/using-branches)

### Overwrite master with empty project

```sh
git branch -D master
git checkout --orphan master
git rm -rf .
git commit --allow-empty -m "Initial commit"
git merge another-master --allow-unrelated-histories
git push origin master -f
```

### Tag commit and push it

```bash
git tag v1.7.7-beta.20 d43bab9
git push origin master --tags
```

### How to check number of commits by person

```bash
git shortlog -s -n | head -n 20
```

### How to change https to ssh authorization in existing repo

Open file `config` from `.git` folder in you project repository: `code /project_name/.git/config`.

Change url address from one to another.

### Show linked remote repository

```sh
git remote show origin
```

### Change linked remote repository

From https to ssl for example.

```sh
ssh://git@domain.com:7999/project_name
```

### How to revert specific Merge

```sh
git fetch origin
git checkout origin/feature/name-of-branch -b feature/name-of-branch
git revert -m 1 b76a5f1f5d3b323679e466a1a1d
```

## Bash

### ZSH and oh-my-zsh - Make bash more intuitive and usefull

> ZSH also called the Z shell, is an extended version of the Bourne Shell (sh), with plenty of new features, and support for plugins and themes. Since it???s based on the same shell as Bash, ZSH has many of the same features, and switching over is a breeze.

Install `ZSH` and `Oh-My-ZSH` (freamwork for easly manage zsh - additional plugins and themes):

```Bash
brew install zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)" #install Oh-My-ZSH
```

### Add auto suggestions and shell syntax highlight

You have to install two plugins: `zsh-autosuggestions` and `zsh-syntax-highlighting`.

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
vim ~/.zshrc
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

Now, you can add it to your zsh config file `~/.zshrc`.

```bash
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
```

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
