# Berkshelf
[![Code Climate](https://codeclimate.com/badge.png)](https://codeclimate.com/github/RiotGames/berkshelf)

Manage a Cookbook or an Application's Cookbook dependencies

## Installation

    $ gem install berkshelf

## Usage

See [berkshelf.com](http://berkshelf.com) for up-to-date usage instructions.

# Contributing

## Running tests

### Install prerequisites

Install the latest version of [Bundler](http://gembundler.com)

    $ gem install bundler

Clone the project

    $ git clone git://github.com/RiotGames/berkshelf.git

and run:

    $ cd berkshelf
    $ bundle install

Bundler will install all gems and their dependencies required for testing and developing. 

### Running unit (RSpec) and acceptance (Cucumber) tests

Simply copy the `spec/knife.rb.sample` to `spec/knife.rb`, and point it at a
chef server. Berkshelf tests may upload and destroy cookbooks on your chef
server, so be sure to configure a server safe for this task.

    $ bundle exec guard start

See [here](https://github.com/tdegrunt/vagrant-chef-server-bootstrap) for a
quick way to get a testing chef server up.

# Authors and Contributors

* Josiah Kiehl (<josiah@skirmisher.net>)
* Jamie Winsor (<jamie@vialstudios.com>)
* Erik Hollensbe (<erik@hollensbe.org>)
* Michael Ivey (<ivey@gweezlebur.com>)
