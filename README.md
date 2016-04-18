BitCurator Custom New User Creation Script
------------------------------------------
<http://wiki.bitcurator.net>

# Getting started


BitCurator New User Creation Script

This script creates new users in the BitCurator environment with full privileges and access to all desktop items originally created for the primary user in the live environment (bcadmin).

# How to use

Open a terminal in BitCurator-1.6.6 or later, and clone out this repository:

 * git clone https://github.com/bitcurator/bitcurator-adduser

Change directory into the new bitcurator-adduser directory, and run:

 * sudo ./bcadduser -u USERNAME

where USERNAME is the name of the new user you wish to create. The username must not include any spaces.

# Warning

The BitCurator environment was originally designed for live and single-user use only. Use this script at your own risk. It has basic checks to examine the system for existing users and prevent accidentally overwriting such a user. 

This script modifies the sudoers file with new entries equivalent to the existing bcadmin user. This means that any new users you add will have full administrative privileges on the system, just as the bcadmin user does.