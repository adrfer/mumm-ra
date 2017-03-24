# Mumm-Ra
Transform your decayed machine into an awesome development one.

Tested against `GNU bash 3.2.57` and `Git 2.10.1`.

## Usage

Open a terminal and run:

    bash <(curl -sL https://raw.github.com/adrfer/mumm-ra/master/transform)

Mumm-Ra can be run as many times as needed on the same machine safely. Installs, upgrades, and/or skips are based on what's already setup. So, no worries!

## Customize

### The `transform` script

Feel free to review and modify the `transform` script to better suit your needs.

By default, the script sets up:

- [homebrew](http://brew.sh)
- [tree](http://mama.indstate.edu/users/ice/tree)
- [wget](http://www.gnu.org/software/wget)
- [vim](http://www.vim.org)
- [tmux](http://tmux.github.io)
- [unrar](http://www.rarlab.com)
- [rbenv](http://github.com/sstephenson/rbenv)
- [ruby-build](https://github.com/sstephenson/ruby-build)
- [ruby](http://www.ruby-lang.org)
- [shellcheck](http://www.shellcheck.net)
- [rubygems](http://rubygems.org)
- [bundler](http://bundler.io)

### The `~/.mumm-ra.local` file

To further customize your setup, put whatever you need at the `~/.mumm-ra.local` file. An example file is provided with this repository.

--
**Note:** Mumm-Ra wouldn't exist if it wasn't for awesome prior art. It's been inspired by thoughtbot's great [laptop](https://github.com/thoughtbot/laptop) project.

--
Hey, looking for some bash badassery? Check out [bash-oh-my](https://github.com/adrfer/bash-oh-my).

Interested in tuning your git profile? Take a look at [git-oh-my](https://github.com/adrfer/git-oh-my).
