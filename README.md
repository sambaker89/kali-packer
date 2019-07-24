# Kali Mini

## Description

* Rolling KALI linux (https://www.kali.org/)
* Built for KVM
* Build QCOW2 image files from ISO
* libvirt/kvm installed on host

## Setup the PACKER environment (in the execution shell)

```
 export PACKER_LOG="1"
 export PACKER_LOG_PATH='./logs/packerlog.txt'
```
## Directory tree Setup

```
kali_packer
  logs
  box
  tmp
  http
```

## Qemu location

* qemu-system-x86_64 executable in Centos 7 is qemu-kvm
* file location: /usr/libexec/qemu-kvm
* add the iteam "qemu_binary" to the kali.json

## Usage

 ```
 packer build -var "version=0.1" -var disk_size=60345 kali.json
 ```

## Notes
* disable any extra DHCP server on the KVM
* ensure only one active DHCP network interface

## References

* https://github.com/tsondt/kali-mini-rolling-packer-vagrant
* https://github.com/offensive-security/kali-linux-preseed
