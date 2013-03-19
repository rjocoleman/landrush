# 
# This serves as a simple example, and it's what I'm using for testing locally.
#
# If you're doing development and want to run this locally you can simply
# `bundle install`, then prefix all your vagrant commands with `bundle exec`, like so:
#
#   bundle exec vagrant up
#   bundle exce vagrant halt
#

# This line is unnecessary when the plugin is installed normally; it's just
# here for the development / testing use case.
Vagrant.require_plugin "vagrant-rubydns"

Vagrant.configure("2") do |config|
  config.vm.box = "precise64"

  config.vm.provision :rubydns

  config.vm.network :private_network, ip: '172.16.32.111'

  config.vm.hostname = "myhost.vagrant.dev"
end