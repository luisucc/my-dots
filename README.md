# dots

![image](https://i.cloudup.com/RCpB-ASfme.png)

WIP bootstrapping library for osx & ubuntu (and maybe others!)

My dots repository, taken from [https://github.com/pierrelepair](https://github.com/pierrelepair), original repo/author is: [https://github.com/matthewmueller/dots](https://github.com/matthewmueller/dots) not forked to not mess up everybody's network graph for now.

## Installation

One-liner:

Currently, no such thing, please `git clone` this project and check it out.
You may afterwards run.

```
sh dots.sh boot osx
```


<!-- ```
(mkdir -p /tmp/dots && cd /tmp/dots && curl -L https://github.com/gato-omega/my-dots/archive/master.tar.gz | tar zx --strip 1 && sh ./install.sh)
```
 -->
## Design

The goal of dots is to automate the process of getting your operating system from a stock build to a fully functional machine.

Dots should be the first thing you download and run to get your computer set up.

This library tries to be organized like a node application, while working within the constraints of bash.

## Supported Operating systems:

### Mac OS X

The OSX build does the following:

- install homebrew
- installs binaries (graphicsmagick, python, sshfs, ack, git, etc.)
- sets OSX defaults (seems taken from [https://gist.github.com/brandonb927/3195465](https://gist.github.com/brandonb927/3195465))
- installs applications via `homebrew-cask` (one-password, sublime-text, virtualbox, nv-alt, iterm2, etc.)
- sets up the ~/.bash_profile

### Ubuntu (server) (ALPHA)

The Ubuntu build does the following:

- dash => bash
- creates a user
- installs git and curl
- sets up the ssh keys
- configures fail2ban
- sets up the firewall
- installs docker

## TODO

* Consider rewriting to be a cross-compiled Go project
* improve modularity (is there a way to source single functions from files?)
* generalize configuration (use secret gists for configuration)
* git-config
* ubuntu profile
* logging
* much more...

# Credits

* Logo by: [Piotrek Chuchla](http://www.thenounproject.com/pchuchla/)

# License

MIT

Taken from [https://github.com/pierrelepair](https://github.com/pierrelepair).
Original author/repo at: [https://github.com/matthewmueller/dots](https://github.com/matthewmueller/dots)

Not forked to not mess up everybody's network graph for now.
