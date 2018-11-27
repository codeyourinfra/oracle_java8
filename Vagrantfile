# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "generic/alpine38"

  config.vm.provision "shell", inline: <<-SHELL
    # https://wiki.alpinelinux.org/wiki/Installing_Oracle_Java
    apk --no-cache --allow-untrusted -X https://apkproxy.herokuapp.com/sgerrand/alpine-pkg-glibc add glibc glibc-bin
    mkdir -p /opt/java
    cd /opt/java
    curl -L -b "oraclelicense=a" http://download.oracle.com/otn-pub/java/jdk/8u191-b12/2787e4a523244c269598db4e85c51e0c/jdk-8u191-linux-i586.tar.gz -O
    sudo tar -zxvf jdk-8u191-linux-i586.tar.gz
    ln -s /opt/java/jdk1.8.0_191 /opt/java/current
    echo "export JAVA_HOME=/opt/java/current" > /etc/profile.d/java.sh
    echo 'export PATH=$PATH:$JAVA_HOME/bin' >> /etc/profile.d/java.sh
    source /etc/profile.d/java.sh
    #apk add paxctl
    #cd jdk1.8.0_191/bin
    #paxctl -c java
    #paxctl -m java
    #paxctl -c javac
    #paxctl -m javac
  SHELL
end
