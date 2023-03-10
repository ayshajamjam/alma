# [Alma](https://almasaasproj.herokuapp.com/)

## About

Alma is a SaaS app that allows students to create and sign up for tasks within their own school community.<br />

## Demo

<a href="https://youtu.be/j8B8YcH2qHk" target="_blank"><img src="./Homepage.png" 
alt="demo video" width="550" height="300" border="10" /></a>

Visit our demo video [here](https://youtu.be/j8B8YcH2qHk) <br />
Visit our Heroku page [here](https://almasaasproj.herokuapp.com/) (this link is expired)

## Group members
Aditi Dam - ad3707 <br/>
Aysha Jamal - aj2604 <br/>
Elizabeth Walker - ejw2173 <br/>
Vanessa Vasquez - vv2317 

## Set up
- Run 'bundle install'
- Run 'rake db:seed'
- Run 'rake db:migrate'

## Set up mailcatcher in development
1) Run 'gem install mailcatcher'
2) If 1) gave you errors, run the following: gem install mailcatcher -- --with-cflags="-Wno-error=implicit-function-declaration"
3) Run 'mailcatcher'
4) Run 'bundle exec rails server'
5) Go to 'http://127.0.0.1:1080/'
6) In another window, sign up for an account on http://localhost:3000/users/sign_up. Make sure to use a university email address that includes .edu
7) Navigate to 'http://127.0.0.1:1080/', and you should see the confirmation email received there!

## Set up heroku 
- Download heroku CLI from website
- Check if downloaded by running 'heroku --version'
- Run 'heroku login' 
- Run 'heroku create'
- Run 'heroku keys:add'
- Run 'git push heroku' 
- Run 'heroku run rake db:migrate'
- Run 'heroku restart'

## To run tests
- Run 'rake cucumber'
- Run 'rspec spec'

## To run project in development
- Run 'bundle exec rails server'

## Notes
- If you want to reseed, run 'rake db:reset' which will drop the data, migrate, and reseed.
- If still in development mode, load mailcatcher to approve seeded users
