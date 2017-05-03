# Install a web development machine

This repo contains scripts to set up an OS X or Linux computer for web 
development, and to keep it up to date.

It can be run multiple times on the same machine safely. It installs,
upgrades, or skips packages based on what is already installed on the machine.

## Install

In your Terminal window, copy and execute the command below.

```sh
bash <(curl -s https://raw.githubusercontent.com/laupiFrpar/web-development-machine/master/web-development-machine)
```

**Once the script is done, quit and relaunch Terminal.**

It is highly recommended to run the script regularly to keep your computer up
to date. Once the script has been installed, you'll be able to run it at your
convenience by typing `web-development-machine`.

## What it sets up

* [Homebrew] for managing operating system libraries
* [Homebrew Cask] for quickly installing Mac apps from the command line
* [Homebrew Services] so you can easily stop, start, and restart services
* [Textmate 2] for coding all the things
* [Firefox] for testing your Rails app on a browser other than Chrome or Safari
* [iTerm2] - an awesome replacement for the OS X Terminal
* [Git] - a CVS tool
* [Bash Completion] - a completion tool for bash
* [Sass] - an extension of CSS that adds power and elegance to the basic language
* [PHP] - a popular scripting language
* [Composer] - a dependency manager for PHP

[Homebrew]: http://brew.sh/
[Homebrew Cask]: http://caskroom.io/
[Homebrew Services]: https://github.com/Homebrew/homebrew-services
[Textmate 2]: https://macromates.com/
[Firefox]: https://www.mozilla.org/en-US/firefox/new/
[iTerm2]: http://iterm2.com/
[Git]: https://git-scm.com/
[Bash Completion]: https://github.com/scop/bash-completion
[Sass]: https://rubygems.org/gems/sass
[PHP]: https://secure.php.net/
[Composer]: https://getcomposer.org/

It should take less than 15 minutes to install (depends on your machine and
internet connection).

```bash
cd ~
curl --remote-name https://raw.githubusercontent.com/tomislav/osx-terminal.app-colors-solarized/master/Solarized%20Dark.terminal
curl --remote-name https://raw.githubusercontent.com/tomislav/osx-terminal.app-colors-solarized/master/Solarized%20Light.terminal
open Solarized%20Dark.terminal
open Solarized%20Light.terminal
```

This will add the Solarized themes to your Terminal's Profiles, and if you want to set one of them as the default, go to your Terminal's Preferences, click on the Settings tab, scroll down to the Solarized Profile, click on it, then click the Default button. When you open a new window or tab (or if you quit and relaunch Terminal), it will use the Solarized theme.

## Credits

This laptop script is inspired by
[monfresh's laptop](https://github.com/monfresh/laptop) script.

## Todo

- Customize installation
  - Customize PS1
- Replace values instead of append at the end of file `append_to_file`
- Install textmate's plugins
- Install Docker