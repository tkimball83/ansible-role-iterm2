# ansible-role-iterm2

[![Build Status](https://travis-ci.org/tkimball83/ansible-role-iterm2.svg?branch=master)](https://travis-ci.org/tkimball83/ansible-role-iterm2)

macOS - Terminal Replacement

## Requirements

This role requires homebrew and homebrew cask to be installed

## Role Variables

Available variables are listed below, along with default values:

    iterm2_pkg: iTerm2
    iterm2_domain: "com.googlecode.{{ iterm2_pkg|lower }}"
    iterm2_defaults: {}

## Dependencies

None

## Example Playbook

    - hosts: localhost
      connection: local
      roles:
        - role: tkimball83.iterm2
          iterm2_defaults:
            OnlyWhenMoreTabs:
              type: string
              value: 0
            PromptOnQuit:
              type: bool
              value: false

## License

GPLv3

## Author Information

This role was created by [Taylor Kimball](http://www.linuxhq.org).
