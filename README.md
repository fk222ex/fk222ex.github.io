# Jekyll Boilerplate

This is a boilerplate to be used for Jekyll-assignments in the course. The virtual machine (Ubuntu 32bit) will have the following (relevant) packages installed:
* node.js (Latest stable)
* npm
* git 
* bundler

## Install
Make sure you have the following installed on your system:
* Virtual Box [https://www.virtualbox.org/](https://www.virtualbox.org/)
* Vagrant [https://www.vagrantup.com/](https://www.vagrantup.com/)

Now, do:

1. Pull (`git pull https://github.com/1dv022/jekyll-boilerplate.git`) into your existing repo. Make sure you are in the root of your repo.

2. Start the virtual machine using `vagrant up` (Will take 15-30 minutes. Ignore red command line statements and warnings.)

3. SSH into the machine using  `vagrant ssh`

4. Change directory to `cd /vagrant`

5. Install depencies and github-pages `npm install` (Will run bundle install postinstallation)

6. Create an scaffolded jekyll project using `jekyll new src` (`src` to install in the directory (`/vagrant/src`)

## Daily workflow
1. Start out by `vagrant up` your machine and ssh into it (`vagrant ssh`). Change directory to `cd /vagrant`.

2. Start watching for changes in the jekyll files. `npm run watch`

3. Open up a browser and visit the url `http://localhost:4000`

4. Fire up the IDE of your choise (Webstorm, sublime etc.) and open the files in the `src`-folder and start editing your site. When a file is saved the watch-script will auto generate the site. (including sass-files)

5. When you are done simply `ctrl+c` to abort the watch, `exit` to  exit the ssh-session and do a `vagrant halt` to stop the machine or `vagrant suspend` to only suspend it.
