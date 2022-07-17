# rtw8852be
Linux driver for RTW8852BE PCIe card


### Software Packages to be installed

```bash

sudo dnf upgrade
sudo dnf install dkms make kernel-devel -y
sudo dnf install @development-tools dkms
sudo dnf install kernel-headers kernel-devel
sudo dnf groupinstall "Development Tools"
sudo dnf groupinstall "C Development Tools and Libraries"
sudo dnf install lsb_release
sudo dnf install linux-headers bcc
sudo dnf install clang llvm go make libbpf-devel bpftool -y

sudo dnf install dwarves
```

#### Install from repo
make sure to disable secure boot before installing

```
sudo make -j8
sudo make install

sudo modprobe 8852be
```

###### To Clean
```bash
sudo make clean
```