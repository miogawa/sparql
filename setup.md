Set up fuseki
===

Presetup
---
0. configuration
macbook pro os x 10.9.2  2.4 GHz Intel Core i5  8GB 1600 MHz DDR3

1. Downloads
 - [virtual box](https://www.virtualbox.org)
 - [cent os](http://www.centos.org) 

2. Set up virtual box with cent os
  1. install virtual box
  2. click **new** and create virtual machine
    1. choose linux redhat
      - memory 2GB, fixed hdd 12GB, NAT and Host only adapter
    2. first time starting virtual machine choose cent os iso image file you download.
      - choose language as japanese, webserver type 
      - add Firefox, KDE, and X-system from custom package.

> first time setting Host only adapter, need to add adapter.
 1. choose **virtual box** from top bar
 2. **preferance** -> **network** -> **Host-only networks**
 3. add adapter

Set up guest os(cent os virtual machine)
---
0. configuration
centos 6.5

1. Downloads
 - [Apache Jena fuseki](http://jena.apache.org/download/index.cgi)
 - ruby # yum install ruby

2. Open and start fuseki
 1. tar xzvf jena-fuseki-1.0.1-distribution.tar.gz
 2. mv -r jena-fuseki-1.0.1 /usr/lib/fuseki
 3. cd /usr/lib/fuseki
 4. chmod +x fuseki-server s-*
 5. export PATH=$PATH:/usr/lib/fuseki
 6. fuseki-server --update --mem /ds

  

