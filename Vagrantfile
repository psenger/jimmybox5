# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

    config.vm.box = "sternpunkt/jimmybox-5"
    config.vm.network "private_network", ip: "192.168.33.12"
    config.vm.hostname = "jimmy5"
    config.vm.synced_folder ".", "/var/www", :mount_options => ["dmode=777", "fmode=666"]

    # SHOPWARE Developers:
    # you should try NFS share instead of the upper synced folder. It performs much better!
    # config.vm.synced_folder "./", "/var/www", :nfs => { :mount_options => ["dmode=777","fmode=666"] }

end
