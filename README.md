# zookeeper-debian-packaging

https://packages.debian.org/experimental/zookeeper

http://ftp.de.debian.org/debian/pool/main/z/zookeeper/zookeeper_3.4.6-3.dsc
http://ftp.de.debian.org/debian/pool/main/z/zookeeper/zookeeper_3.4.6.orig.tar.xz
http://ftp.de.debian.org/debian/pool/main/z/zookeeper/zookeeper_3.4.6-3.debian.tar.xz

cd build
tar xvf ../zookeeper_3.4.6-3.debian.tar.xz

update debian/changelog
debuild -S -sa -k0FF66C63 (twice?)
dput ppa:serverdensity/zookeeper  ../zookeeper_3.4.6-5_source.changes

