#!/usr/bin/env ruby
# -*- mode: ruby -*-
# vi: set ft=ruby :

require "vagrant-librarian-chef"

Vagrant.configure("2") do |config|
  config.vm.box = "chef/ubuntu-14.04"

  config.omnibus.chef_version = '11.16.4'

  config.vm.provision :chef_solo do |chef|
    chef.cookbooks_path = "cookbooks"
    chef.add_recipe "git"
  end
end
