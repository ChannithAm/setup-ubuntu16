# Setup Ubuntu
=================

## . Update & Upgrade

```
sudo apt-get update
sudo apt-get -y upgrade
```

## . install git

```
sudo apt-get git
sudo apt-get install git bash-completion
```
Detail click (here)[https://github.com/ChannithAm/Git-command]

## . Install Java

```
sudo add-apt-repository ppa:webupd8team/java
sudo apt-get update
sudo apt-get install oracle-java8-installer
```

Install Eclipse:
-----------------
```
sudo add-apt-repository ppa:ubuntu-desktop/ubuntu-make
sudo apt update
sudo apt install ubuntu-make
umake ide eclipse
```



=======================================================

## . Common Errors

E: Could not get lock /var/lib/apt/lists/lock - open Resource temporarily unavailable

```
sudo rm -rf  /var/lib/apt/lists/lock
```
-------------------------------------------------------
user@plato:~# apt-get update
0% [Connecting to us.archive.ubuntu.com (2001:67c:1562::14)] [Connecting to sec░

change line ~54 to uncomment the following
```
sudo vim /etc/gai.conf
precedence ::ffff:0:0/96  100
```

**Caution** Look out line 50 looks almost indentical:
```
precedence ::ffff:0:0/96  10
```

--------------------------------------------------------
E: Package 'vim' has no installation candidate
```
sudo apt-get update
sudo apt-get install vim
```

##. References

[1] https://itsfoss.com/install-latest-eclipse-ubuntu/
