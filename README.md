The DataTank vagrant setup
==========================

This repository contains a [Vagrant](http://www.vagrantup.com/) setup for [The DataTank](http://thedatatank.com/).
The goal of this setup is to try out The DataTank and build stuff on top of it.

## Prerequisite

Make sure you have [vagrant](http://docs.vagrantup.com/v2/installation/) and [VirtualBox](https://www.virtualbox.org/wiki/Downloads) installed on your machine.

## Installation

```bash
git clone https://github.com/metaodi/datatank-vagrant.git
cd datatank-vagrant
vagrant up
```

### Host entry

In order to be able to easily access your vagrant box, you should add the following entry to your hosts file (usually `/etc/hosts`)

```bash
172.23.5.42    datatank.lo
```

After doing that you'll be able to access your own installation of The DataTank using the following URL: http://datatank.lo

### Load test data

By default, no test data is loaded. To do that, simply run the following command:

```bash
vagrant provision testdata
```
