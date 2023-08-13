ansible [core 2.14.6]
Vagrant 2.3.7

docker image used is 'ip2backend-docker'

![Alt text](image-1.png)

# DNS Container
Server:    10.96.0.10
Address 1: 10.96.0.10 kube-dns.kube-system.svc.cluster.local

Name:      web-0.nginx
Address 1: 10.244.0.11 web-0.nginx.default.svc.cluster.local

# application is scaled up 5 times and persisted
NAME        STATUS   VOLUME                                     CAPACITY   ACCESS MODES   STORAGECLASS   AGE
www-web-0   Bound    pvc-371a5b13-5e0c-4a98-a745-19ba913415c0   1Gi        RWO            standard       40m
www-web-1   Bound    pvc-9d522000-dbf9-4752-9ea1-e36ea3f83ef7   1Gi        RWO            standard       38m
www-web-2   Bound    pvc-4be0907a-5abd-40df-97d0-ddcb13f2bf19   1Gi        RWO            standard       3m17s
www-web-3   Bound    pvc-efa057b5-d8ba-4446-af3d-554b1eb51383   1Gi        RWO            standard       3m14s
www-web-4   Bound    pvc-a06e510c-6f11-4d27-8105-df2a4f12e6b4   1Gi        RWO            standard       3m11s

# Docker images used published
![Alt text](<Screenshot from 2023-08-13 10-39-47.png>)

![Alt text](<Screenshot from 2023-08-13 10-59-30.png>)