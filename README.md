# ZSOS
- bootloader
- kernel
- shell 

# Docs
[cs wisc](https://pages.cs.wisc.edu/~remzi/OSTEP/)

[os ecci](https://os.ecci.ucr.ac.cr/slides/Abraham-Silberschatz-Operating-System-Concepts-10th-2018.pdf)

[basickernel](https://www.cs.vu.nl/~herbertb/misc/basickernel.pdf)

[linux-insides](https://0xax.gitbooks.io/linux-insides/content/)


# Installations 

1. Build docker the env
```console
$ docker build buildenv -t zosos-buildenv
```

2. Run instance of container on Intel Mac or Windows
```console
Linux / MacOS : docker run --rm -it -v $pwd:/root/env zosos-buildenv
Windows       : docker run --rm -it -v %cd%:/root/env zosos-buildenv
```
3. CD to project dit and command below to create the .iso file in the dist folder.
```console
make build-x86_64
```

4. Install [QEMU](https://qemu.weilnetz.de/w64/) and add to your [path](https://dev.to/whaleshark271/using-qemu-on-windows-10-home-edition-4062#:~:text=2.-,Add%20Qemu%20path%20to%20environment%20variables%20settings,-Copy%20the%20Qemu) then cd to the project dir and run

```console 
qemu-system-x86_64 -cdrom dist/x86_64/kernel.iso
```
