# Sharetribe
## Tech Stack

- Ruby 2.3  
- Ruby on Rails 4.2  
- MySQL  5.7
- React + jQuery
- Node.js 6.9 (for compiling JavaScript assets)
- "what you see is what you get" Editor [Mercury](http://jejacks0n.github.io/mercury/)  
- Deploy: Custom Script (not using Mina or Cap3)  
- Server: Heroku
- Image hosting: Amazon S3  
- Background job: `[delayed_job](https://github.com/collectiveidea/delayed_job)`
- Gem: 
    -  [devise](https://github.com/plataformatec/devise) | Authentication
    -  [omniauth-facebook](https://github.com/mkdynamic/omniauth-facebook) | Third party login: Facebook
    -  [haml](https://github.com/haml/haml) and ERB | HTML teamplating
    -  [mysql2](https://github.com/brianmario/mysql2) | MySQL library for Ruby
    -  [paperclip](https://github.com/thoughtbot/paperclip) | Image upload management
    -  [passenger](https://github.com/phusion/passenger) | Web application server
    -  [react_on_rails](https://github.com/shakacode/react_on_rails) | Integration of React + Webpack + Rails
    -  factory_girl, capybara, rspec-rails, cucumber-rails, selenium-webdriver | Testing

## Installation

### Requirements

Before you get started, the following needs to be installed:
  * **Ruby**. Version 2.3.1 is currently used and we don't guarantee everything works with other versions. If you need multiple versions of Ruby, [RVM](https://rvm.io//) is recommended.
  * [**RubyGems**](http://rubygems.org/)
  * **Bundler**: `gem install bundler`
  * **Node**. Version 6.9 is currently used and we don't guarantee everything works with other versions. If you need multiple versions of Node, consider using [n](https://github.com/tj/n) or [nvm](https://github.com/creationix/nvm).
  * [**Git**](http://help.github.com/git-installation-redirect)
  * **A database**. Only MySQL 5.7 has been tested, so we give no guarantees that other databases (e.g. PostgreSQL) work. You can install MySQL Community Server two ways:
    1. If you are on a Mac, use homebrew: `brew install mysql` (*highly* recommended). Also consider installing the [MySQL Preference Pane](https://dev.mysql.com/doc/refman/5.1/en/osx-installation-prefpane.html) to control MySQL startup and shutdown. It is packaged with the MySQL downloadable installer, but can be easily installed as a stand-alone.
    2. Download a [MySQL installer from here](http://dev.mysql.com/downloads/mysql/)
  * [**Sphinx**](http://pat.github.com/ts/en/installing_sphinx.html). Version 2.1.4 has been used successfully, but newer versions should work as well. Make sure to enable MySQL support. If you're using OS X and have Homebrew installed, install it with `brew install sphinx --with-mysql`
  * [**Imagemagick**](http://www.imagemagick.org). If you're using OS X and have Homebrew installed, install it with `brew install imagemagick`

### Setting up the development environment

brew tap homebrew/versions
brew install v8-315

gem install libv8 -v '3.16.14.13' -- --with-system-v8
gem install therubyracer -- --with-v8-dir=/usr/local/opt/v8-315

bundle install
npm install
