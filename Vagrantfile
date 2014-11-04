# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.define "cozy" do |v|
    v.vm.provider "docker" do |d|
      d.build_dir = "./cozy-setup/"
      d.ports = ['9104:9104']
      d.vagrant_machine = "default"
      d.vagrant_vagrantfile = "./host/Vagrantfile"
      d.force_host_vm = true
      #d.volumes = ['/etc/nginx/sites-available']
    end
  end
end
