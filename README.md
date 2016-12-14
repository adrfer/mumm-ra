# Mumm-Ra
The script that transforms your decayed machine into an awesome development one.

Tested on `GNU bash 3.2.57` and `Git 2.8.4`.

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

Mumm-Ra runs `~/.mumm-ra.local` at the end, so put whatever customizations you might have there.

Here's an example:

```sh
#!/usr/bin/env bash

# Jump to existing directory or create it
jump() {
  [[ "${#}" = 1 ]] || {
    echo 'Usage: jump PATH'
    return 1
  }
  
  [[ -n "${1}" ]] && mkdir -p "${1}"
  cd "${1}"
}
```

--
**Note:** Mumm-Ra wouldn't exist if it wasn't for awesome prior art. It's been inspired by thoughtbot's great [laptop](https://github.com/thoughtbot/laptop) project.

--
Hey, looking for some bash badassery? Check out [bash-oh-my](https://github.com/adrfer/bash-oh-my).

Interested in tuning your git profile? Take a look at [git-oh-my](https://github.com/adrfer/git-oh-my).
