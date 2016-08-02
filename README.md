# Ubuntu Vagrant VM for Rails Development

## Getting started

1. Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

2. Install [Vagrant](https://www.vagrantup.com/downloads.html)

3. If Windows is the host operating system you will need to set up PuTTY for use with Vagrant or have ssh.exe on your path. See notes below.

4. Clone this repository

    ``` git clone git@github.com:duke-libraries/rails-dev-vagrant.git``` 


5. Change to project directory `cd rails-dev-vagrant`

6. Run `vagrant up`

7. Connect to Vagrant `vagrant ssh`

8. The provisioning script doesn't install java correctly. To install java:

    ```
    vagrant ssh
    sudo add-apt-repository ppa:webupd8team/java
    sudo apt-get update
    sudo apt-get install oracle-java8-installer
    ```

## Using Vagrant on Windows with PuTTY

Follow instructions from: [http://blog.osteel.me/posts/2015/01/25/how-to-use-vagrant-on-windows.html](http://blog.osteel.me/posts/2015/01/25/how-to-use-vagrant-on-windows.html)

1. [Download PuTTY](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html) if don't already have it (the first putty.exe link will do). 
				
2. Download puttygen.exe as well (from the same URL), to get the private key.

3. Load	the private key:
	
    File-> Load private key:

	C:\Users\ad96\TRLN_workspace\rails-dev-vagrant-master\.vagrant\machines\default\virtualbox\private_key
	
	(Adjust path for your username and working directory structure.)

