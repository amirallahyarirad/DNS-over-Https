disable local DNS lisitener on coredns server

edit resolved.conf:

vim /etc/systemd/resolved.conf 
systemctl restart systemd-resolved.service


resolved.conf:

[Resolve]
DNS=8.8.8.8
DNSStubListener=no
