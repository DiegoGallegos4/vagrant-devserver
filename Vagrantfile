# -*- mode: ruby -*-
# vi: set ft=ruby :


Vagrant.configure(2) do |config|
  config.vm.box = "debian-jessie64.box"
  config.vm.network "public_network", bridge: "en0: Wi-Fi (AirPort)"
  #config.vm.network "forwarded_port", guest: 8080, host: 8080
  config.vm.synced_folder "./hrm.panoramalife.com", "/var/www/hrm.panoramalife.com",owner: 'vagrant',  group: 'www-data', mount_options: ["dmode=775,fmode=664"]
  config.vm.synced_folder "./hrm.frontend.dev", "/var/www/hrm.frontend.dev",owner: 'vagrant',  group: 'www-data', mount_options: ["dmode=775,fmode=664"]
  config.vm.synced_folder "./erp.panoramalife.com", "/var/www/erp.panoramalife.com",owner: 'vagrant',  group: 'www-data', mount_options: ["dmode=775,fmode=664"]
end
