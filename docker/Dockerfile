FROM scratch
#ADD openwrt-armvirt-64-default-rootfs.tar.gz /
#ADD openwrt-x86-64-generic-rootfs.tar.gz /
ADD rootfs.tar /
COPY AdGuardHome /usr/bin/AdGuardHome
#COPY turboacc /etc/config/turboacc
COPY dhcp /etc/config/dhcp
COPY firewall /etc/config/firewall
#COPY google_fu_mode /etc/config/google_fu_mode
COPY network /etc/config/network
COPY resolv.conf /root/resolv.conf
COPY rc.local /etc/rc.local
COPY inittab /etc/inittab

EXPOSE 80 443 22

CMD ["/sbin/init"]

