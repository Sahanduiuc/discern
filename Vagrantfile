Vagrant::Config.run do |config|
  config.vm.box = 'ubuntu-12.04.2-i386-chef-11-omnibus'
  config.vm.box_url = 'https://s3.amazonaws.com/gsc-vagrant-boxes/ubuntu-12.04.2-i386-chef-11-omnibus.box'
  config.vm.forward_port 9000, 8000
  
  # http://docs-v1.vagrantup.com/v1/docs/config/vm/share_folder.html
  # config.vm.share_folder "foo", "/guest/path", "/host/path"
  config.vm.share_folder "ml-service-api", "/home/vagrant/ml-service-api", "."
  # setting an IP address with config.vm.network, we can use Fabric to configure the Vagrant box
  config.vm.network :hostonly, "33.33.33.10"
end