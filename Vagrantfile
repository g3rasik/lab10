# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.provider "docker" do |d|
    d.image       = "ubuntu:latest"
    d.name        = "lab10-vagrant-ubuntu"
    d.has_ssh     = false
    d.privileged  = true
    d.cmd         = ["tail", "-f", "/dev/null"]
  end

  config.vm.synced_folder ".", "/vagrant", disabled: true
end
