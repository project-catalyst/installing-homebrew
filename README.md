# Installing Homebrew

Note: This document is a work in progress. If you find yourself here and have suggestions for how to improve it or questions contact me on twitter [@dwesty17](https://twitter.com/dwesty17) or by email at j.dylan.westerhold@gmail.com. I'll do my best to get back to you.

Reading Time: **? minutes**

## Lessons
1. [Using a Command Line Interface](https://github.com/project-catalyst/using-a-cli) (? minutes)
1. **Installing Homebrew**
1. [Running A JavaScript Program](https://github.com/project-catalyst/running-a-javascript-program) (? minutes)
1. [Using Git and GitHub](https://github.com/project-catalyst/overview) (? minutes)
1. [Intro to JavaScript](https://github.com/project-catalyst/overview) (? minutes)
1. [JavaScript Lesson 1: Variables and Data Types](https://github.com/project-catalyst/overview) (? minutes)
1. [JavaScript Lesson 2: Functions](https://github.com/project-catalyst/overview) (? minutes)
1. [JavaScript Lesson 3: Conditional Statements and Loops](https://github.com/project-catalyst/overview) (? minutes)
1. [Intro to React](https://github.com/project-catalyst/overview) (? minutes)

## Overview

[Homebrew](https://brew.sh/) is a package manage for the Mac operating system, which is to say that it's the command line software you will use to install and manage the other command line software on your computer.

## How to Guide

Instructions on how to install Homebrew can be found on their website which is linked to in the section above but they are very simple. Just copy and paste the following command into your terminal window and hit enter.

```shell
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

To confirm that the installation succeeded enter the command `which brew`, which should print out the location on your machine that Homebrew was installed.

```shell
> which brew
/usr/local/bin/brew
```

## First Command to Learn

Homebrew is invoked on the command line by typing `brew` followed by the Homebrew command you want executed and hitting enter.

### install <some software>

Install whichever package you specify after the command, as long as Homebrew knows how to install it. This is likely the Hombrew command you will use most frequently. If Homebrew doesn't know how to install it or has other issues during installation, it will let you know.

```shell
> brew install node
==> Installing dependencies for node: icu4c
==> Installing node dependency: icu4c
==> Downloading https://homebrew.bintray.com/bottles/icu4c-61.1.high_sierra.bottle.tar.gz
######################################################################## 100.0%
==> Pouring icu4c-61.1.high_sierra.bottle.tar.gz
==> Caveats
This formula is keg-only, which means it was not symlinked into /usr/local,
because macOS provides libicucore.dylib (but nothing else).

If you need to have this software first in your PATH run:
  echo 'set -g fish_user_paths "/usr/local/opt/icu4c/bin" $fish_user_paths' >> ~/.config/fish/config.fish
  echo 'set -g fish_user_paths "/usr/local/opt/icu4c/sbin" $fish_user_paths' >> ~/.config/fish/config.fish

For compilers to find this software you may need to set:
    LDFLAGS:  -L/usr/local/opt/icu4c/lib
    CPPFLAGS: -I/usr/local/opt/icu4c/include

==> Summary
🍺  /usr/local/Cellar/icu4c/61.1: 249 files, 67.2MB
==> Installing node
==> Downloading https://homebrew.bintray.com/bottles/node-10.0.0.high_sierra.bottle.tar.gz
######################################################################## 100.0%
==> Pouring node-10.0.0.high_sierra.bottle.tar.gz
==> Caveats
Bash completion has been installed to:
  /usr/local/etc/bash_completion.d
==> Summary
🍺  /usr/local/Cellar/node/10.0.0: 5,301 files, 51.5MB
```

### uninstall <some software>

Uninstalls whichever package you specify after the command, as long as it's installed on your machine and Hombrew knowns how to uninstall it.

```shell
> brew uninstall node
Uninstalling /usr/local/Cellar/node/10.0.0... (5,301 files, 51.5MB)
```

## Next Lesson

[Running a JavaScript Program](https://github.com/project-catalyst/running-a-javascript-program)