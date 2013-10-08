*Currently being edited*

Ruby on Rails Workshop
===

Table of Contents
---

1. [Ruby Tutorials](#-1-ruby-tutorials)
2. [Development Machine Setup](#-2-development-machine-setup)
    * [Windows](#-windows)
    * [Linux](#-linux)

<a id="ruby-tutorials"></a> 1. Ruby Tutorials
---

Following tutorials are amazing.

* [tryruby](http://tryruby.org/levels/1/challenges/0)
* [rubymonk](http://rubymonk.com/)

<a id="development-machine-setup"></a> 2. Development Machine Setup
---

### <a id="setup-windows"></a> Windows
1. Install Ruby on Rails
  
  [RailsInstaller](http://railsinstaller.org/en "Install ruby, rails git and other tools")


2. Install Editor [Sublime Text 3](http://www.sublimetext.com/3)

  [http://www.sublimetext.com/3](http://www.sublimetext.com/3)


### <a id="setup-linux"></a> Linux

Following instructions are taken from [http://gorails.com/setup/ubuntu](http://gorails.com/setup/ubuntu)

1. Install Ubuntu 13.04 (64-bit if your machine is 64-bit) Ask friends who have already install ubuntu. Before installing another operating system do backup your data to external hard drive incase you loose anything.

  [http://www.ubuntu.com/download/desktop](http://www.ubuntu.com/download/desktop)

  Following are two [Dual Boot](http://en.wikipedia.org/wiki/Multi_boot) tutorials I found.
  
  [Windows 7 with Ubuntu 13.04](https://www.youtube.com/watch?v=SeSaVzyPY8k)

  [Windows 8 with Ubuntu 13.04](https://www.youtube.com/watch?v=PK7gWIkAY7s)

2. Open [terminal](https://help.ubuntu.com/community/UsingTheTerminal) in ubuntu and run the following commands, update package manager
> ```
sudo apt-get update
> ```

3. Install libraries
> ```
sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev \
libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt-dev
> ```


3. Go to [home directory](http://en.wikipedia.org/wiki/Home_directory#Unix)
> ```
cd
> ```

4. Install [rbenv](https://github.com/sstephenson/rbenv)
> ```
git clone git://github.com/sstephenson/rbenv.git .rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL
> ```

5. Install ruby-build
> ```
git clone git://github.com/sstephenson/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL
> ```

6. Install [ruby](https://en.wikipedia.org/wiki/Ruby_(programming_language)
> ```
rbenv install 2.0.0-p247
rbenv global 2.0.0-p247
ruby -v
> ```

7. When [gems](http://en.wikipedia.org/wiki/RubyGems "in ruby libraries are called gems rails is also a gem") are installed no need to install documentation.
> ```
echo "gem: --no-ri --no-rdoc" > ~/.gemrc
> ```

8. Create a github account if you don't have one.

  [https://github.com](https://github.com)

  [https://help.github.com](https://help.github.com)

8. Setup [git](https://git.com)/[github](https://github.com), use your account info
> ```
git config --global color.ui true
git config --global user.name "Wasim Akram"
git config --global user.email "xxxxxxxx@gmail.com"
ssh-keygen -t rsa -C "xxxxxxxx@gmail.com"
> ```

9. Show the generated ssh key
> ```
cat ~/.ssh/id_rsa.pub
> ```

10. Copy the printed ssh key and paste in to the following link

  [https://github.com/settings/ssh](https://github.com/settings/ssh)

11. Verify Github you should see response similar to "Hi excid3! You've successfully authenticated, but GitHub does not provide shell access."
> ```
ssh -T git@github.com
> ```

12. Install [nodejs](http://nodejs.org/)
> ```
sudo add-apt-repository ppa:chris-lea/node.js
sudo apt-get update
sudo apt-get install nodejs
> ```

13. Install [rails](http://guides.rubyonrails.org/)
> ```
gem install rails
> ```

14. Rehash rbenv so it will pick up install rails
> ```
rbenv rehash
> ```

15. Verify rails its version should be 4.0.0+
> ```
rails -v
> ```

16. Create a new rails application
> ```
rails new myapp
> ```

17. Change directory to myapp
> ```
cd myapp
> ```

18. Create Database
> ```
rake db:create
> ```

19. Start the server
> ```
> rails server
> ```

20. Verify Application works

  [http://localhost:3000](http://localhost:3000)

21. Install Editor [Sublime Text 3](http://www.sublimetext.com/3)

  [http://www.sublimetext.com/3](http://www.sublimetext.com/3)