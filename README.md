# OpenBSD Packer Templates

![](https://i.imgur.com/waxVImv.png)
### [View all Roadmaps](https://github.com/nholuongut/all-roadmaps) &nbsp;&middot;&nbsp; [Best Practices](https://github.com/nholuongut/all-roadmaps/blob/main/public/best-practices/) &nbsp;&middot;&nbsp; [Questions](https://www.linkedin.com/in/nholuong/)
<br/>

This repository contains templates for building OpenBSD boxes for
[Vagrant](http://www.vagrantup.com) using [Packer](http://packer.io).
Supports VirtualBox, VMware, and QEMU/libvirt providers.

Pre-built boxes can be installed via [Hashicorp Atlas](https://atlas.hashicorp.com/search?q=ryanmaclean%2Fopenbsd):

Current:

```
vagrant box add ryanmaclean/openbsd-6.1
```

Older:

```
vagrant box add ryanmaclean/openbsd-6.0
```

You can also build the boxes yourself:
```
packer build openbsd-<version>.json
```

The boxes won't include VirtualBox Guest Additions nor VMware Tool
(as they are not available for the OS). So for synced folders you need to use
e.g. [NFS](https://docs.vagrantup.com/v2/synced-folders/nfs) or
[rsync](https://docs.vagrantup.com/v2/synced-folders/rsync).

## Chef and Ansible Support

The images created by this script currently support Chef and/or Ansible installation at build time. 

### Chef
In order to have Chef installed in the Vagrant box, set `chef_version` (line 3) to either `prerelease` or `latest` in the json file for the version you are building. 

### Ansible
In order to have Ansible installed in the Vagrant box, set `vagrant_ansible` (line 8) to `yes` in the json file for your build. 

# 🚀 I'm are always open to your feedback.  Please contact as bellow information:
### [Contact ]
* [Name: Nho Luong]
* [Skype](luongutnho_skype)
* [Github](https://github.com/nholuongut/)
* [Linkedin](https://www.linkedin.com/in/nholuong/)
* [Email Address](luongutnho@hotmail.com)
* [PayPal.me](https://www.paypal.com/paypalme/nholuongut)

![](https://i.imgur.com/waxVImv.png)
![](Donate.png)
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/nholuong)

# License