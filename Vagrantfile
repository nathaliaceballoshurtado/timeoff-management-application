Vagrant.configure("2") do |config|
    config.vm.define "jenkins" do |jenkins|
        jenkins.vm.box = "ubuntu/bionic64"
        jenkins.vm.hostname = "jenkins"
        jenkins.vm.provision "ansible" do |ansible|
            ansible.verbose = "v"
            ansible.playbook = "playbook.yaml"
        end
    end
end