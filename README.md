# Ubuntu Vagrant VM for Rails Development

## Getting started

1. Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

2. Install [Vagrant](https://www.vagrantup.com/downloads.html)

3. Clone this repository

4. Run `vagrant up`.

5. (Optional) The provisioning script doesn't install java correctly. To install java:

    ```
    vagrant ssh
    sudo add-apt-repository ppa:webupd8team/java
    sudo apt-get update
    sudo apt-get install oracle-java8-installer
    ```
