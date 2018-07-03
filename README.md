# Kali Mini

## What

* Small Kali linux (https://www.kali.org/)
* Built for KVM
* Minimal kali linux rolling
* Produces a vagrant box (https://www.vagrantup.com/)
* libvirt/kvm installed on host

##  tl;dr

```
root/vagrant
```

## Qemu location

* qemu-system-x86_64 executable in Centos 7 is qemu-kvm
* file location: /usr/libexec/qemu-kvm
* add the iteam "qemu_binary" to the kali.json

## References

* https://github.com/tsondt/kali-mini-rolling-packer-vagrant
* https://github.com/offensive-security/kali-linux-preseed
