Laptop
======

Laptop is a script to set up a macOS laptop for web and mobile development.

It can be run multiple times on the same machine safely.
It installs, upgrades, or skips packages
based on what is already installed on the machine.

Requirements
------------

We support:

* macOS Mavericks (10.9)
* macOS Yosemite (10.10)
* macOS El Capitan (10.11)
* macOS Sierra (10.12)
* macOS High Sierra (10.13)
* macOS Mojave (10.14)

Older versions may work but aren't regularly tested.
Bug reports for older versions are welcome.

Install
-------

1. Log into iTunes, iCloud, App Store
2. Install XCode dev tools: `xcode-select --install`
2. Download the script:

```sh
curl -LOk https://github.com/cema-sp/laptop/archive/master.zip
```

Review the script (avoid running scripts you haven't read!):

```sh
unzip -a master.zip
cd ./laptop-master
less mac
```

Execute the downloaded script:

```sh
sh mac 2>&1 | tee ./laptop.log
```

Optionally, review the log:

```sh
less ~/laptop.log
```

[dotfiles]: https://github.com/thoughtbot/dotfiles#install

What it sets up (to be updated)
---------------

macOS tools:

* [Homebrew] for managing operating system libraries.

[Homebrew]: http://brew.sh/

Unix tools:

* [Git] for version control
* [OpenSSL] for Transport Layer Security (TLS)
* [RCM] for managing company and personal dotfiles
* [The Silver Searcher] for finding things in files
* [Tmux] for saving project state and switching between projects
* [Zsh] as your shell

[Git]: https://git-scm.com/
[OpenSSL]: https://www.openssl.org/
[RCM]: https://github.com/thoughtbot/rcm
[The Silver Searcher]: https://github.com/ggreer/the_silver_searcher
[Tmux]: http://tmux.github.io/
[Zsh]: http://www.zsh.org/

Heroku tools:

* [Heroku CLI] for interacting with the Heroku API

[Heroku CLI]: https://devcenter.heroku.com/articles/heroku-cli

GitHub tools:

* [Hub] for interacting with the GitHub API

[Hub]: http://hub.github.com/

Image tools:

* [ImageMagick] for cropping and resizing images

Programming languages, package managers, and configuration:

* [Bundler] for managing Ruby libraries
* [Node.js] and [NPM], for running apps and installing JavaScript packages
* [Ruby] stable for writing general-purpose code
* [Yarn] for managing JavaScript packages

[Bundler]: http://bundler.io/
[ImageMagick]: http://www.imagemagick.org/
[Node.js]: http://nodejs.org/
[NPM]: https://www.npmjs.org/
[Ruby]: https://www.ruby-lang.org/en/
[Yarn]: https://yarnpkg.com/en/
