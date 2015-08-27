Rails 4.2.4
Ruby 2.2.3p173
mysql 

===============================================================================================
Create VagrantApp
create folder MyDocuments/VagrantApp
create folder MyDocuments/Projects

 -cd VagrantApp
 -vagrant init lvphu609/lucid32
 
config file Vagrantfile
	config.vm.network :forwarded_port, guest: 3000, host: 3000
	
 -vagrant up
 -vagrant ssh

 ~$ sudo apt-get update
 ~$ sudo apt-get install build-essential git-core sqlite3
 ~$ git clone https://github.com/sstephenson/rbenv.git ~/.rbenv
 ~$ echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile
 ~$ echo 'eval "$(rbenv init -)"' >> ~/.bash_profile
 ~$ source .bash_profile
 ~$ git clone git://github.com/sstephenson/ruby-build.git
 ~$ cd ruby-build/
 ~/ruy-build$ sudo ./install.sh
 ~/ruy-build$  rbenv install 2.2.3
 ~/ruy-build$  rbenv rehash
 ~/ruy-build$  rbenv global 2.2.3

 -cd /vagrant
create folder vagrant_data
create new project rails or coppy project rails existed to vagrant_data folder
 -cd vagrant_data 
 -gem install bundler
 -gem install rails
 -rbenv rehash
 
view rails version
	-rails -v
	
Install Mysql
  -sudo apt-get install mysql-server
	-sudo netstat -tap | grep mysql
	(if not run sudo service mysql restart)



====================================================
NOTE
virturbox store on 
  https://atlas.hashicorp.com/lvphu609 
or search on link http://www.vagrantbox.es/ 

vagrant doc https://www.vagrantup.com/
