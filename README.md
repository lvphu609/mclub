Rails 4.2.4 <br>
Ruby 2.2.3p173 <br>
mysql 

<p><strong>Create VagrantApp</strong></p>

<ol>
	<li>
	<p>create folder MyDocuments/VagrantApp</p>
	</li>
	<li>
	<p>create folder MyDocuments/Projects</p>
	</li>
	<li>
	<p><strong>cd VagrantApp</strong></p>
	</li>
	<li>
	<p><strong>vagrant init lvphu609/lucid32</strong></p>
	</li>
	<li>
	<p>config file Vagrantfile</p>
	</li>
</ol>

<p><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; config.vm.network :forwarded_port, guest: 3000, host: 3000</strong></p>

<p>&nbsp; &nbsp; &nbsp;6.&nbsp;<strong>vagrant up</strong></p>

<p>&nbsp; &nbsp; &nbsp;7. <strong>vagrant ssh</strong></p>

<p>&nbsp; &nbsp; &nbsp;8.<br />
<strong>&nbsp;~$ sudo apt-get update</strong></p>

<p><strong>~$ sudo apt-get install build-essential git-core sqlite3</strong></p>

<p><strong>~$ git clone https://github.com/sstephenson/rbenv.git ~/.rbenv</strong></p>

<p><strong>~$ echo &#39;export PATH=&quot;$HOME/.rbenv/bin:$PATH&quot;&#39; &gt;&gt; ~/.bash_profile</strong></p>

<p><strong>~$ echo &#39;eval &quot;$(rbenv init -)&quot;&#39; &gt;&gt; ~/.bash_profile</strong></p>

<p><strong>~$ source .bash_profile</strong></p>

<p><strong>~$ git clone git://github.com/sstephenson/ruby-build.git</strong></p>

<p><strong>~$ cd ruby-build/</strong></p>

<p><strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ~/ruy-build$ sudo ./install.sh</strong></p>

<p><strong>~/ruy-build$ &nbsp;rbenv install 2.2.3</strong></p>

<p><strong>~/ruy-build$ &nbsp;rbenv rehash</strong></p>

<p><strong>~/ruy-build$ &nbsp;rbenv global 2.2.3</strong></p>

<p>&nbsp;</p>

<p>&nbsp; &nbsp; &nbsp;9.&nbsp;<strong>cd /vagrant</strong></p>

<p>&nbsp; &nbsp; &nbsp;10. create folder vagrant_data</p>

<p>&nbsp; &nbsp; &nbsp;11.<strong>&nbsp;</strong>create new project rails or coppy project rails existed to vagrant_data folder</p>

<p>&nbsp; &nbsp; &nbsp;12. <strong>cd vagrant_data </strong></p>

<p>&nbsp; &nbsp; &nbsp;13.&nbsp;<strong>gem install bundler</strong></p>

<p>&nbsp; &nbsp; &nbsp;14. <strong>gem install rails</strong></p>

<p>&nbsp; &nbsp; &nbsp;15. <strong>rbenv rehash</strong></p>

<p>&nbsp; &nbsp; &nbsp;16. view rails version</p>

<p><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; rails -v</strong></p>

<p>&nbsp; &nbsp; &nbsp; 17. <strong>sudo apt-get install mysql-server</strong></p>

<p><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; sudo netstat -tap | grep mysql</strong></p>

<p><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; </strong>&nbsp;(if not run sudo service mysql restart)</p>

<p><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; </strong>&nbsp; username root</p>

<p>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; password 123456</p>

<p>&nbsp;</p>

<p>&nbsp; &nbsp; &nbsp; &nbsp;18.</p>

<p><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;sudo apt-get install libmysqlclient-dev</strong></p>

<p><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;gem install mysql2</strong></p>

<p><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</strong> &rArr; fix not install gem install mysql2</p>

<p>&nbsp;</p>

<p>&nbsp; &nbsp; &nbsp; &nbsp;19. add to Gemfile</p>

<p><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;gem &#39;therubyracer&#39; </strong></p>

<p><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;gem &#39;execjs&#39;</strong></p>

<p>&nbsp;</p>

<p><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;</strong> &nbsp; and run</p>

<p><strong>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; bundle install</strong></p>

<p>&nbsp;</p>

<p><strong>=&gt; fix javascript run time. Nodejs</strong></p>

<p><br />
&nbsp;</p>

<p><strong>====================================================</strong></p>

<p><strong>NOTE</strong></p>

<p><strong>virturbox store on <a href="https://atlas.hashicorp.com/lvphu609">https://atlas.hashicorp.com/lvphu609</a> or search on link <a href="http://www.vagrantbox.es/">http://www.vagrantbox.es/</a> </strong></p>

<p>&nbsp;</p>

<p><strong>vagrant doc <a href="https://www.vagrantup.com/">https://www.vagrantup.com/</a></strong></p>


