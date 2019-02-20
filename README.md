# ansible-mysqldump

Simple mysqldump script for ansible. Can customize exporting of database by defining a regular expression and/or explicit list of tables to copy. Will export db scheme only and/or scheme and data based on configuration.


## Requirements

* mysqldump installed locally
* gz compress lib

## Usage

### Example Playbook

- hosts: server
  become: yes
  vars_files:
    - vars/main.yml
  roles:
    - { role: kxlops.mysqldump }


## Release Notes

v .01 - Initial test release

## Road Map

* look at integrating S3 buckets
* look at implementing '--skip-extended-insert'

