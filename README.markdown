#Fedena : Open source school management system

Project Fedena is the open source school management system based on Ruby on Rails. It is developed by a team of developers at Foradian Technologies. The project was made open source by Foradian, and is now maintained by the open source community. Fedena is the ideal solution for schools and campuses that want an easy means to manage all campus records.

The Project Fedena website http://www.projectfedena.org/ is the home to the developer community behind Fedena project. There you can find forums and bug tracker for Fedena.

#Demo
A demo website for Fedena has been set up at demo.projectfedena.org. You can log in with following usernames and passwords:

    * As admin -- username - admin, password - admin123
    * As student -- username - 1, password - 1123
    * As employee -- username - E1, password - E1123

#License

Fedena is released under the Apache License 2.0.

#Installation

Visit  http://projectfedena.org/install for detailed installation instruction.

#Community Support:

Visit www.projectfedena.org for community support.

#Tweaked for an OS X dev machine

I tweaked the code a little in order to run it in an OS X 10.8.4 Mac. Merged the [code](http://projectfedena.org/download/fedena-bundle-linux) linked in [here](http://projectfedena.org/install) with the code from the original github repo.

##Requirements
  * [Homebrew](http://brew.sh/)
  * [RVM](http://rvm.io) with [autolibs on](https://rvm.io/rvm/autolibs)
  
## Commands
This guide assumes you cloned this repo into a `fedena` directory. `$` is the bash prompt.

  ```bash
    $ brew install mysql
  ```
  
  Configure MySQL user according to *your* settings in the config/database.yml file.
  
  ```bash
    $ rvm install 1.8.7
    $ cd fedena/
    $ rvm use 1.8.7@fedena --create --ruby-version
    $ rvm rubygems 1.3.7
    $ bundle install --local
  ```

  ```bash
    $ rake db:create
    $ rake fedena:plugins:install_all
    $ chmod +x script/*
    script/server
  ```
  
  ;-)
