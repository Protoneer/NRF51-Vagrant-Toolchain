# Vagrant Basic Ubuntu Box Template

## Introduction
Vagrant is a tool for building virtual workspaces. Its main benifits is that work enviroments can be setup once and destributed between users. Perfect for sharing complex Toolchains. This repository provides the `vagrantfile` that contains all the enviroment settings to create the virtual linux box that can compile [mBed GCC projects](https://developer.mbed.org/handbook/Exporting-to-GCC-ARM-Embedded).

## Requirements
* [Vagrant](https://www.vagrantup.com/downloads.html)
* [Virtualbox](https://www.virtualbox.org/wiki/Downloads)

## Install
All that is needed to create the virtual box is to run `vagrant up` in the folder containing the `vagrantfile`

After the installation has been done the a SSH port will be opened on the local host with the following details.
* SSH 127.0.0.1:2222
* Username : vagrant
* Password : vagrant

A shared folder is also create:
On the Linux box folder `/vagrant` is the same as the host folder where the `vagrantfile` is located.

## Usage
* Download this repository to a local folder.
* SSH to the Vagrant box (SSH details above)(I use Putty for windows and SSH for Linux)
* `cd /vagrant` (Shared folder with the host)
