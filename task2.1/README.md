# Task 2.1
## VirtualBox
![alt text](https://github.com/LawRider/DevOps_online_Kharkiv_2021Q2/blob/master/task2.1/1.png)
![alt text](https://github.com/LawRider/DevOps_online_Kharkiv_2021Q2/blob/master/task2.1/2.png)
![alt text](https://github.com/LawRider/DevOps_online_Kharkiv_2021Q2/blob/master/task2.1/3.png)
![alt text](https://github.com/LawRider/DevOps_online_Kharkiv_2021Q2/blob/master/task2.1/4.png)
![alt text](https://github.com/LawRider/DevOps_online_Kharkiv_2021Q2/blob/master/task2.1/5.png)
![alt text](https://github.com/LawRider/DevOps_online_Kharkiv_2021Q2/blob/master/task2.1/6.png)
![alt text](https://github.com/LawRider/DevOps_online_Kharkiv_2021Q2/blob/master/task2.1/7.png)
![alt text](https://github.com/LawRider/DevOps_online_Kharkiv_2021Q2/blob/master/task2.1/8.png)
![alt text](https://github.com/LawRider/DevOps_online_Kharkiv_2021Q2/blob/master/task2.1/9.png)
## Vagrant
![alt text](https://github.com/LawRider/DevOps_online_Kharkiv_2021Q2/blob/master/task2.1/10.png)
> [02:55 AM] alex /mnt/1000 $ vagrant init hashicorp/precise64
> A `Vagrantfile` has been placed in this directory. You are now
> ready to `vagrant up` your first virtual environment! Please read
> the comments in the Vagrantfile as well as documentation on
> `vagrantup.com` for more information on using Vagrant.
> [02:57 AM] alex /mnt/1000 $ less Vagrantfile
> [02:57 AM] alex /mnt/1000 $ vagrant up
> Bringing machine 'default' up with 'virtualbox' provider...
> ==> default: Importing base box 'hashicorp/precise64'...
> ==> default: Matching MAC address for NAT networking...
> ==> default: Checking if box 'hashicorp/precise64' version '1.1.0' is up to date...
> ==> default: Setting the name of the VM: 1000_default_1616461079950_86101
> Vagrant is currently configured to create VirtualBox synced folders with
> the `SharedFoldersEnableSymlinksCreate` option enabled. If the Vagrant
> guest is not trusted, you may want to disable this option. For more
> information on this option, please refer to the VirtualBox manual:
>
>   https://www.virtualbox.org/manual/ch04.html#sharedfolders
>
> This option can be disabled globally with an environment variable:
>
>   VAGRANT_DISABLE_VBOXSYMLINKCREATE=1
>
> or on a per folder basis within the Vagrantfile:
>
>   config.vm.synced_folder '/host/path', '/guest/path', SharedFoldersEnableSymlinksCreate: false
> ==> default: Clearing any previously set network interfaces...
> ==> default: Preparing network interfaces based on configuration...
>     default: Adapter 1: nat
> ==> default: Forwarding ports...
>     default: 22 (guest) => 2222 (host) (adapter 1)
> ==> default: Booting VM...
> ==> default: Waiting for machine to boot. This may take a few minutes...
>     default: SSH address: 127.0.0.1:2222
>     default: SSH username: vagrant
>     default: SSH auth method: private key
>     default:
>     default: Vagrant insecure key detected. Vagrant will automatically replace
>     default: this with a newly generated keypair for better security.
>     default:
>     default: Inserting generated public key within guest...
>     default: Removing insecure key from the guest if it's present...
>     default: Key inserted! Disconnecting and reconnecting using new SSH key...
> ==> default: Machine booted and ready!
> ==> default: Checking for guest additions in VM...
>     default: The guest additions on this VM do not match the installed version of
>     default: VirtualBox! In most cases this is fine, but in rare cases it can
>     default: prevent things such as shared folders from working properly. If you see
>     default: shared folder errors, please make sure the guest additions within the
>     default: virtual machine match the version of VirtualBox you have installed on
>     default: your host and reload your VM.
>     default:
>     default: Guest Additions Version: 4.2.0
>     default: VirtualBox Version: 6.1
> ==> default: Mounting shared folders...
>     default: /vagrant => /mnt/1000
> [02:58 AM] alex /mnt/1000 $ ssh vagrant@127.0.0.1 -p 2222
> Warning: Permanently added '[127.0.0.1]:2222' (ECDSA) to the list of known hosts.
> vagrant@127.0.0.1's password:
> Welcome to Ubuntu 12.04 LTS (GNU/Linux 3.2.0-23-generic x86_64)
>
>  * Documentation:  https://help.ubuntu.com/
> New release '14.04.6 LTS' available.
> Run 'do-release-upgrade' to upgrade to it.
>
> Welcome to your Vagrant-built virtual machine.
> Last login: Fri Sep 14 06:23:18 2012 from 10.0.2.2
> vagrant@precise64:~$ date
> Tue Mar 23 01:01:00 UTC 2021
> vagrant@precise64:~$ logout
> Shared connection to 127.0.0.1 closed.
> [03:01 AM] alex /mnt/1000 $ vagrant halt
> ==> default: Attempting graceful shutdown of VM...
> [03:01 AM] alex /mnt/1000 $ vagrant destroy
>     default: Are you sure you want to destroy the 'default' VM? [y/N] y
> ==> default: Destroying VM and associated drives...
> [03:02 AM] alex /mnt/1000 $
