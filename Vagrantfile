Vagrant.configure("2") do |config|
    config.vm.define "main" do |config|
        config.vm.box = "archlinux/archlinux"
        config.vm.synced_folder ".", "/vagrant"

        config.ssh.username = "vagrant"
        config.ssh.password = "vagrant"

        config.vm.provider "virtualbox" do |vb|
            vb.name = "workstation-dev"
        end
    end
end