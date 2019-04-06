![Logo](https://github.com/BitCurator/bitcurator.github.io/blob/master/logos/BitCurator-Basic-400px.png)

# BitCurator environment custom new user creation script

[![GitHub issues](https://img.shields.io/github/issues/bitcurator/bitcurator-distro-adduser.svg)](https://github.com/bitcurator/bitcurator-distro-adduser/issues)
[![GitHub forks](https://img.shields.io/github/forks/bitcurator/bitcurator-distro-adduser.svg)](https://github.com/bitcurator/bitcurator-distro-adduser/network)
[![Build Status](https://travis-ci.org/BitCurator/bitcurator-distro-adduser.svg?branch=master)](https://travis-ci.org/BitCurator/bitcurator-distro-adduser)
[![Twitter Follow](https://img.shields.io/twitter/follow/bitcurator.svg?style=social&label=Follow)](https://twitter.com/bitcurator)

## DEPRECATION NOTICE:

This repository has been deprecated, and is no longer maintained. Details on the latest release can be found at (https://github.com/bitcurator/bitcurator-distro). The most recent Salt-based build repository can be found at (https://github.com/bitcurator/bitcurator-distro-salt).

## Getting started

This script creates new users in the BitCurator environment with full privileges and access to all desktop items originally created for the primary user in the live environment (bcadmin).

## How to use

Open a terminal in BitCurator-1.6.6 or later, and clone out this repository:

```shell
git clone https://github.com/bitcurator/bitcurator-adduser
```

Change directory into the new bitcurator-adduser directory, and run:

```shell
sudo ./bcadduser -u USERNAME
```

where USERNAME is the name of the new user you wish to create. The username must not include any spaces.

## Warning

The BitCurator environment was originally designed for live and single-user use only. Use this script at your own risk. It has basic checks to examine the system for existing users and prevent accidentally overwriting such a user. 

This script modifies the sudoers file with new entries equivalent to the existing bcadmin user. This means that any new users you add will have full administrative privileges on the system, just as the bcadmin user does.

## License(s)

The BitCurator logo, BitCurator project documentation, and other non-software products of the BitCurator team are subject to the the Creative Commons Attribution 4.0 Generic license (CC By 4.0).

Unless otherwise indicated, software items in this repository are distributed under the terms of the GNU General Public License, Version 3. See the text file "COPYING" for further details about the terms of this license.

In addition to software produced by the BitCurator team, BitCurator packages and modifies open source software produced by other developers. Licenses and attributions are retained here where applicable.
