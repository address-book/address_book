# Address Book

A simple web app for showing off your testing

This application is deployed to: https://address-book-example.herokuapp.com/

## Local Installation

You can also create a local instance of this app. Local builds are currently only supported for MacOS or Linux. 

First you will need to have 

- Ruby 2.4.1 installed (using the helpful [`rbenv`](https://github.com/rbenv/rbenv) if required)
- Bundler (which can be installed by `gem install bundle`)
- PostgreSQL (which can be installed on Mac using `brew install postgresql` or Linux using something like `sudo apt-get install postgresql`)
- Rails (which can be installed by `gem install rails`).

Once you have these prequesites in place, you can create a local build by executing
```
bundle install;
rails s
```
As part of these build steps, you may also need to migrate the existing database. This can be done by executing
```
rails db:migrate RAILS_ENV=development
```
and rerunning `rails s`.

If the app is built successfully, the app will be found at `http://localhost:3000`.