## Overview

KOBman, is a command line utility which gives you a `kob` command on your shell, you can use it to automate the setup of various development environments required for [projects](./sub_projects.md) under KochiOrgBook.


## Installing KOBman using oah-shell

We will be using [oah-installer](https://github.com/hyperledgerkochi/oah-installer), a component of [**OpenAppHack(OAH)**](https://openapphack.github.io/OAH/), to install [oah-shell](https://github.com/hyperledgerkochi/oah-shell) in the local system and using it to bring up [oah-kob-vm](https://github.com/hyperledgerkochi/oah-kob-vm) with KOBman installed.

## Pre-requisites

- <a href="https://www.virtualbox.org/" target="_blank">Virtual Box</a>
- <a href="https://www.vagrantup.com/" target="_blank">Vagrant</a>
- <a href="https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html" target="_blank">Ansible</a>

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

</br></br>


Check out the demo video

<iframe src="https://player.vimeo.com/video/562887067?autoplay=1&loop=1&autopause=0" width="700" height="500" frameborder="0" allow="fullscreen; autoplay"></iframe>
</br></br></br>
<center>
<a href="https://github.com/hyperledgerkochi/KOBman" target="_blank" title="Source Code"><svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" viewBox="0 0 16 16"><defs><style>svg:hover {fill: blue;}</style></defs><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"/></svg></a></br>
<caption>Source Code</caption>
<center>
<!-- ## Demo video

Take a look at the <a href="https://vimeo.com/562887067" target="_blank">Demo Video</a>.

## Source code

Source code for .
 -->
