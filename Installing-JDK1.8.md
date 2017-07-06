# Windows
* Go to this page: http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
* Under **Java SE Development Kit 8u121** click to accept the license agreement
* Download the windows `.exe` for your operating system (32 bit or 64 bit)
* Use the `.exe` to install

# Linux
* Open your terminal (or ssh into your server)
* Run the following commands. You may need to remove the `sudo` at the beginning if running as root:
```
sudo add-apt-repository ppa:webupd8team/java
sudo apt-get update
sudo apt-get install oracle-java8-installer
```

# Raspberry Pi
* Open your terminal (or ssh into your pi)
* Run the following commands:
```
sudo apt-get update
sudo update-alternatives --config java
```
* Select Oracle JDK 1.8, then run:
```
sudo update-alternatives --config javac
```
* Select Oracle JDK 1.8

# Mac
* Go to this page: http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
* Under **Java SE Development Kit 8u121** click to accept the license agreement
* Download the mac `.dmg`
* Use the `.dmg` to install