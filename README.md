# pluralsight-js-dev-env
Pluralsight tutorial for creating a JavaScript Development Environment

- Setup generic vagrant box:
  - on host:
    - new vagrant box:
      $ vagrant init ubuntu/trusty64; vagrant up --provider virtualbox
      $ vagrant ssh
      - I had to increase memory to 1024
  - on guest:
    - install node via nvm:
      $ sudo apt-get update
      $ sudo apt-get install build-essential libssl-dev
      $ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.0/install.sh | bash
      $ nvm install --lts
      $ nvm ls
      $ nvm alias default lts/*
    - install ruby via rvm:
      $ gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
      $ \curl -sSL https://get.rvm.io | bash -s stable
      $ rvm use ruby --install --default

- Tutorial:
  $ npm install
  - security check:
    $ npm install -g nsp
    $ nsp check
    - todo: add to nmp start


