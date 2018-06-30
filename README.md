# ansible-role-iterm2

[![Build Status](https://travis-ci.org/tkimball83/ansible-role-iterm2.svg?branch=master)](https://travis-ci.org/tkimball83/ansible-role-iterm2)
[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-iterm2-blue.svg?style=flat)](https://galaxy.ansible.com/tkimball83/iterm2)
[![License](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](COPYING)

macOS - Terminal Replacement

## Requirements

This role requires homebrew and homebrew cask to be installed

## Role Variables

Available variables are listed below, along with default values:

    iterm2_defaults: {}
    iterm2_domain: "com.googlecode.{{ iterm2_package|lower }}"
    iterm2_package: iTerm2

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

Copyright (C) 2018 Taylor Kimball <tkimball@linuxhq.org>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.
