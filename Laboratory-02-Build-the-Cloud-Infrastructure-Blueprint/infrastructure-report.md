# Infrastructure Report

## Checkpoint 2 – Cloud Server Investigation

The information was collected from the KillerCoda Linux environment:

| Item | Finding |
|---|---|
| Operating System | Ubuntu 24.04.4 LTS (Noble Numbat) |
| Kernel Version | 6.8.0-138-generic |
| CPU Model | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| CPU Cores | 1 |
| Total RAM | 1.9 GiB |
| Disk Capacity | 19 GB |
| Mounted File Systems | `/`, `/boot`, `/boot/efi`, `/run`, `/dev/shm`, `/run/lock` |
| Hostname | ubuntu |
| IP Address | 172.30.1.2, 172.17.0.1 |

## Commands Used

cat /etc/os-release
uname -r
lscpu
nproc
free -h
df -h
df -hT
hostname
hostname -I
