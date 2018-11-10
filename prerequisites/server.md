# Server

## **Getting a Server**

You will need a dedicated server, from a server provider \(e.g. Hetzner, kimsufi, OVH, etc\), installed with Ubuntu Server [16.04](http://releases.ubuntu.com/16.04/) or [18.04](http://releases.ubuntu.com/18.04/).

_Note 1: Cloudbox only supports x64 \(i.e. Intel or AMD 64\) machines. ARM based hardware is not supported._

_Note 2: If you are using a Scaleway server, read_ [_this_](https://github.com/Cloudbox/Cloudbox/wiki/FAQ#if-you-are-using-a-scaleway-server)_._

_Note 3: If you are setting this up on a home server, make sure you open the relevant_ [_ports_](https://github.com/Cloudbox/Cloudbox/wiki/Reference%3A-Cloudbox-Ports) _\(eg `80`, `443`, etc\) in your_ [_router_](https://portforward.com/router.htm)_/firewall, before installing Cloudbox._

_Note 4: If using Ubuntu Desktop, make sure SSH is enabled._

## Tips

### Ubuntu

#### 16.04

* If given an option like below, choose the one with the `HWE Kernel`.

  ![](https://camo.githubusercontent.com/e254894c727e7240b62e1278f6b25228ac0c6438/68747470733a2f2f692e696d6775722e636f6d2f6e4243734439452e706e67)

* If you get an option like below, select choose `ubuntu-1604-xenial-64-minimal`.

  ![](https://camo.githubusercontent.com/0d4edc80e77917ce7e3a37f42b97861a6e6bfc33/68747470733a2f2f692e696d6775722e636f6d2f44635a4141574d2e706e67)

#### 18.04

* If you get an option like below, select choose `ubuntu-1804-beaver-64-minimal`.

  ![](https://camo.githubusercontent.com/0d4edc80e77917ce7e3a37f42b97861a6e6bfc33/68747470733a2f2f692e696d6775722e636f6d2f44635a4141574d2e706e67)

### Partitioning

* If you have multiple hard drives on the server \(eg. 2 x 4 TB\), put them in RAID 0 to maximize space and speed \(you don't need redundancy as you can schedule backups of Cloudbox\).
* Set all available space to `/` \(remove `/home` and `/data` partitions\).
* Leave ample space in `/boot` \(e.g. 2+ GB\).
* Examples
  * Online.net

    ![](https://camo.githubusercontent.com/41dca2353eeaec84cafefb30ccdaca942ade1649/68747470733a2f2f692e696d6775722e636f6d2f3172444373347a2e706e67)

  * OVH

    ![](https://camo.githubusercontent.com/1d5acd3194dc6384815f0527789926e8086c6e70/68747470733a2f2f692e696d6775722e636f6d2f4752546a5176742e706e67)

    ![](https://camo.githubusercontent.com/7daec846c60e6ad368dbdf8de1f16a6c62cba9a4/68747470733a2f2f692e696d6775722e636f6d2f557152324743762e706e67)

