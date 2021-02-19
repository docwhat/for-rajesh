# frozen_string_literal: true

# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure('2') do |config|
  config.vm.box = 'ubuntu/focal64'
  config.vm.define 'alice' { |machine| machine.vm.hostname = 'alice' }
  config.vm.define 'bob' { |machine| machine.vm.hostname = 'bob' }

  # Create a private "Host-Only" network with a second NIC.
  config.vm.network 'private_network', type: 'dhcp', adapter: 2
end
# EOF
