# linux on mac

want to run linux in a virtual machine on your macbook? you are in the right place.

there are two dependencies you need to install:
1. qemu
2. vagrant
```
brew install qemu
brew tap hashicorp/tap
brew install hashicorp/tap/hashicorp-vagrant
```

then use `cd` to the linux distro directory you want to use, and run `vagrant up`.

```
cd ubuntu
vagrant up && vagrant ssh
$ uname -a
Linux ubuntu 5.15.0-76-generic #83-Ubuntu SMP Thu Jun 15 19:21:56 UTC 2023 aarch64 aarch64 aarch64 GNU/Linux

vagrant halt           # to stop
vagrant destroy        # to completely remove
```
