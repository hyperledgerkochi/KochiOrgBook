## Overview

KOBman, is a command line utility which gives you a `kob` command on your shell, you can use it to automate the setup of various development environments required for [projects](./sub_projects.md) under KochiOrgBook.

## Installing KOBman using oah-shell

We will be using [oah-installer](https://github.com/hyperledgerkochi/oah-installer), a component of [**OpenAppHack(OAH)**](https://openapphack.github.io/OAH/), to install [oah-shell](https://github.com/hyperledgerkochi/oah-shell) in the local system and using it to bring up a [oah-kob-vm](https://github.com/hyperledgerkochi/oah-kob-vm) with KOBman installed.

## Pre-requisites

- [Virtual Box](https://www.virtualbox.org/)
- [Vagrant](https://www.vagrantup.com/)
- [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

## Installation

1. Open your terminal 

2. Execute the below command to set the correct namespace

        export OAH_NAMESPACE=hyperledgerkochi

3. Install oah-shell

        curl -L https://raw.githubusercontent.com/hyperledgerkochi/oah-installer/master/install.sh | bash

4. Confirm the installation oah-shell by executing the below command which would list various oah commands

        oah

5. Execute the below command to get the list of environments 

        oah list

    Note: Make sure **oah-kob-vm** is listed. If not, execute step 2 and run the below command

        source ${OAH_DIR}/bin/oah-init

6. Setup oah-kob-vm for KOBman by executing the below command.

        oah install -v oah-kob-vm

## Testing

1. Install an environment

        kob install -env [environment_name] -V [version]

    Run the below command to get the list of available enviornments

        kob list

2. Uninstall an environment

        kob uninstall -env [environment_name] -V [version]

## Demo video

Take a look at the [demo video](https://vimeo.com/562887067).

## Source code

Source code for [KOBman](https://github.com/hyperledgerkochi/KOBman)

