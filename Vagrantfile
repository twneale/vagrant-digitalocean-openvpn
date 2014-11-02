# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "digital_ocean"
  config.vm.provider :digital_ocean do |provider, override|
      override.ssh.private_key_path = './id_rsa'
      provider.token = ENV["DIGITAL_OCEAN_TOKEN"]
      provider.image = ENV["DIGITAL_OCEAN_IMAGE"]
      provider.region = ENV["DIGITAL_OCEAN_REGION"]
      provider.size = ENV["DIGITAL_OCEAN_SIZE"]
  end
end
