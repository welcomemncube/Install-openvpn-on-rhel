# Installing openvpn on RHEL 8

## Install the following packages first:
` dnf install libnl3-devel`  
` dnf install libcap-ng-devel pkgconfig`   
` dnf install lz4-devel`  
` dnf install lzo-devel`  
` dnf install pam-devel` 
` sudo dnf install openvpn`
https://www.looklinux.com/how-to-upgrade-openssl-on-rhel-and-centos-operating-systems/
ln -s libssl.so.3 libssl.so
sudo ldconfig
echo "/usr/local/lib64" > /etc/ld.so.conf.d/openssl.conf

## Then download the tar file from the official OpenVPN site:  
https://openvpn.net/community-downloads/  
` tar -xvf openvpn-2.6.6.tar.gz`  
` cd openvpn-2.6.6`  
` make`  
` make install`
https://community.openvpn.net/openvpn/wiki/OpenvpnSoftwareRepos


