# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...


Reddit:

git init

git status

git add .

git commit -am "Initial Commit"

git checkout -b link_scaffold

rails g scaffold Link title:string url:string

git commit -am "Generate Link Scaffold"

git checkout master

git merge link_scaffold

git checkout -b add_users


rails g devise:install

rails g devise User

rails db:migrate

rails c {
User.count
@user = User.first

}

git status

git add .

git commit -am "Add devise and create User model"


rails g migration add_user_id_to_links user_id:integer:index

rails db:migrate

git status

git add .

git commit -am "Add  assosietion between link and user"

git status

git add .

git commit -am "Authorization on links"

git checkout master

git merge add_users

git checkout -b add_bootstrap

git status

git add .

git commit -am "Add stacture and basic styling"

user1@gmail.com
123456


time:=>00:40:10