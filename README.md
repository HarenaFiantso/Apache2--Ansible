# __APACHE 2 x ANSIBLE__

We used to create VirtualHosts manually with a bash script before. This time, we will do it automatically using a script in a .yaml file with __ANSIBLE__.

<br><br>
## 1. FIRST STEP: INSTALLATION
_APACHE INSTALLATION_:

The first thing we need to do is to install __APACHE2__ in our operating system (I'm using Manjaro in this case):

```shell
sudo pacman -Sy
sudo pacman -S apache

# or

pamac install apache

# or

yay -S apache
```

If Apache is already installed on our system, then great. To check if it's installed, you can run the following command (for ArchLinux-based operating systems):

```shell
# Check the version.
httpd -v

# If Apache is installed, you will see the Apache version displayed in the terminal output. If it doesn't display anything, then you need to run the command above.
```

_ANSIBLE INSTALLATION_:

To install __ANSIBLE__ on Manjaro, you can follow the steps below:

```shell
sudo pacman -S ansible
```

Once the installation is complete, you should have __ANSIBLE__ installed on your Manjaro system.
<br>

You can verify if __ANSIBLE__ is installed by running the following command to display the Ansible version:

```shell
ansible --version

# or

pacman -Q | grep ansible
```

This should display information about the installed version of Ansible on your system.

Now, you can use Ansible to automate configuration and deployment tasks on your target hosts.
