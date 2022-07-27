# Zsos
- bootloader
- kernel
- shell 

# Docs
[cs wisc](https://pages.cs.wisc.edu/~remzi/OSTEP/)

[os ecci](https://os.ecci.ucr.ac.cr/slides/Abraham-Silberschatz-Operating-System-Concepts-10th-2018.pdf)

[basickernel](https://www.cs.vu.nl/~herbertb/misc/basickernel.pdf)

[linux-insides](https://0xax.gitbooks.io/linux-insides/content/)

# Order of ops 
1. 
2. 
3. 
4. 
5.  

# Installations 

Build docker the env
```console
$ docker build buildenv -t zosos-buildenv
```

Run instance of container on Intel Mac or Windows

Linux / MacOS : docker run --rm -it -v $pwd:/root/env zosos-buildenv
Windows       : docker run --rm -it -v %cd%:/root/env zosos-buildenv
