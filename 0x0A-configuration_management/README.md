# Configuration management
* DevOps  SysAdmin	Scripting	CI/CD

## Concepts
* Intro to Configuration Management
* Puppet resource type: file (check “Resource types” for all manifest types in the left menu)
* Puppet’s Declarative Language: Modeling Instead of Scripting
* Puppet lint
* Puppet emacs mode

## Requirements
* Files will be interpreted on Ubuntu 20.04 LTS
* Puppet manifests must pass puppet-lint version 2.1.1 without any errors
* Puppet manifests must run without error
* Your Puppet manifests files must end with the extension .pp

## Note on Versioning
Ubuntu 20.04 VM should have Puppet 5.5 preinstalled.

### Install puppet
$ apt-get install -y ruby=1:2.7+1 --allow-downgrades
$ apt-get install -y ruby-augeas
$ apt-get install -y ruby-shadow
$ apt-get install -y puppet

### Install puppet-lint
$ gem install puppet-lint

## Tasks :page_with_curl:

* **0. Create a file**
  * [0-create_a_file.pp](./0-create_a_file.pp): Puppet manifest file that
  creates a file `school` in the `/tmp` directory.
    * File permissions: `0744`.
    * File group: `www-data`.
    * File owner: `www-data`.
    * File content: `I love Puppet`.

* **1. Install a package**
  * [1-install_a_package.pp](./1-install_a_package.pp): Puppet manifest file
  that install `flask` from pip3.

* **2. Execute a command**
  * [2-execute_a_command.pp](./2-execute_a_command.pp): Puppet manifest file
  that kills the process `killmenow`.
