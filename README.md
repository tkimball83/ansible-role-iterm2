# ansible-role-iterm2

[![Build Status](https://travis-ci.org/tkimball83/ansible-role-iterm2.svg?branch=master)](https://travis-ci.org/tkimball83/ansible-role-iterm2)

macOS - Terminal Replacement

## Requirements

This role requires Homebrew and Homebrew Cask to be installed

## Role Variables

Available variables are listed below, along with default values:

    iterm2_pkg: iTerm2
    iterm2_domain: "com.googlecode.{{ iterm2_pkg|lower }}"
    iterm2_plist: {}

## Dependencies

  * https://galaxy.ansible.com/geerlingguy/homebrew

## Example Playbook

    - hosts: servers
      roles:
        - role: tkimball83.iterm2
          iterm2_plist:
            OnlyWhenMoreTabs:
              type: string
              value: 0
            PromptOnQuit:
              type: bool
              value: false

## License

BSD

## Author Information

This role was created by [Taylor Kimball](http://www.linuxhq.org).
