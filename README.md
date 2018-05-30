# A Recipe for a HAProxy 1.8 stable version RPM on CentOS

Perform the following on a build box as a regular user.

## Install Prerequisites for RPM Creation

    sudo yum groupinstall 'Development Tools'

## Checkout this repository

    cd /opt
    git clone https://github.com/Shocksir/rpm-haproxy.git 
    cd ./rpm-haproxy
    git checkout 1.8

## Build using makefile
    make
    
Resulting RPM will be in /opt/rpm-haproxy/rpmbuild/RPMS/
