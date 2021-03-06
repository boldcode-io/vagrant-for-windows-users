# Vagrant for docker

A ready-for-work environment to run docker + various programming languages with the help of vagrant (and Virtualbox).

It aims to help Windows users which have difficulties running Docker or Unix tools.

## Prerequisites

* Optional : Install [Chocolatey](https://chocolatey.org/install)
* Install Virtualbox (with `choco install virtualbox`)
* Install Vagrant (with `choco install vagrant`)

## Usage

Open Git bash (or Powershell) in the project directory, then run

    $ vagrant up

Once the system is installed, log in onto it by running :

    $ vagrant ssh

Create your ssh keys 

    $ ssh-keygen -f ~/.ssh/myfavorite/project
   
Copy your SSH public key to your source management tool (Github, Bitbucket, Gitlab, whatever...)

Git clone your favorite project in the virtual machine

    $ mkdir -p ~/src
    $ git clone git@somewhere.foo.bar:favorite-project ~/src/favorite-project

And from now on, follow project README or development guidelines :wink:

If you need to work with Visual Studio editor and run commands within the linux box
you can also follow this guide : [Connect Visual Studio Code with Vagrant in your local machine](https://medium.com/@lopezgand/connect-visual-studio-code-with-vagrant-in-your-local-machine-24903fb4a9de)


## References

* [Automating developer machine setup with Chocolatey](https://octopus.com/blog/automate-developer-machine-setup-with-chocolatey)
