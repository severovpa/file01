Vagrant.configure("2") do |config|
  config.vm.box = "bento/debian-8.11-i386"
  config.vm.box_check_update = false
   # config.disksize.size = "15GB"

  config.vm.provider "virtualbox" do |vb|
    # ��� ����������� ������
    vb.name = "debian8-01test"
    # ����� ����������� ������
    vb.memory = 2048
    # ������ �������� �����
    # vb.customize ["modifyhd", :id, "--resize", "10240"]
    # ���������� ���� ����������
    vb.cpus = 2
  end

  # hostname ����������� ������ 
  config.vm.hostname = "debian8-01test"

  config.vm.provision "shell", path: "provision.sh"


end
