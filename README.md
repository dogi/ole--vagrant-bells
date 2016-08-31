# ole--vagrant-bells

ole--vagrant-bells gives users the ability to quickly install their own community [BeLL](https://github.com/open-learning-exchange/BeLL-Apps) (Basic e-Learning Library) on their computer. 

## Requirements
- Install [git](https://git-scm.com/downloads)
  - [Git](https://git-scm.com) is an open source version control system that we use for communication and management for our software. More specifically, we use gitter.im for communication and github.com for software management.
  - Confirmed working on v2.5.0 (check with `git --version`)
- Install [virtualbox](https://www.virtualbox.org/wiki/Downloads)
  - [Virtualbox](https://www.virtualbox.org) allows you to install a software virtualization package as an application on your OS. 
  - Confirmed working on v5.0.14 (check with `vboxmanage --version`)
- Install [vagrant](https://www.vagrantup.com/downloads.html)
  - [Vagrant](https://www.vagrantup.com) is an open source tool for building development environments. 
  - Confirmed working on v1.8.1 (check with `vagrant --version`)
 
### Ubuntu
```sh
    sudo apt-get install git
    sudo apt-get install virtualbox
    sudo apt-get install vagrant
```

### OSX
Open your `Terminal`. We assume that [brew](http://brew.sh/) is already installed.
```sh
    brew install git 
    brew cask install vagrant
    brew cask install virtualbox
```

### Windows
You need to manually install git, virtualbox, and vagrant via internet from the installation links provided above. To use virtualbox  and Git in the command line you have to make sure they are in your system Path.

Git has 3 options for path evnironment>> 3 options
- The first option is to use Git Bash only. Git commands can only be used with Git Bash. 
- the second option is to run Git from the default Windows command prompt. This will add Git to your path.
- the third option is the same as the second one but it also adds unix commands and tools.

The first option is makes the least changes to your system and is the safest option. However, the other two options are more convenient.

![pic](http://i.stack.imgur.com/5szjG.png)


To use virtualbox in the command prompt add vboxmanage to your path. Follow these steps:

- Right click on Computer

- Click on Properties

- Click on Advanced System Settings which opens up a pop up box

- Click on Environment Variables

- Click on Path in the System variables section

- Click Edit System variables

- Click new then browse the directory where your executable is located and click ok

![pic](http://open-learning-exchange.github.io/pages/uploads/images/Environment-Variables.PNG)

Afterwards, open your `Command Prompt` to check that the following are up and running properly:
```sh
git --version
vagrant --version
vboxmanage --version  
```

## Install a communityBeLL on your OS
In your `Terminal` or `Command Prompt`, type:
```sh
git clone https://github.com/dogi/ole--vagrant-bells.git
cd ole--vagrant-bells/release
vagrant up
```

You now have a working [communityBeLL](http://127.0.0.1:5985/apps/_design/bell/MyApp/index.html) on your OS.
