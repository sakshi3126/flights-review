## FlightsReview 
### A flight reviews app built with Ruby on Rails and React.js

This app is intended to be a simple example of a CRUD app built with **Ruby on Rails** and **React.js** using **Webpacker**.

---
![OpenFlights Home](https://github.com/zayneio/open-flights/blob/master/app/assets/images/index-demo.png?raw=true)
---
![OpenFlights Show](https://github.com/zayneio/open-flights/blob/master/app/assets/images/show-demo.png?raw=true)


---

Some of the features of this app include:

* Ruby version: `2.5.3`
* Rails version: `6.0.3`
* Database: `postgresql`
* React version: `16.13.1`
* React Hooks API
* React Context API

## Running it locally
- run `bundle exec rails db:prepare`
- run `npm install` or `yarn install`
- run `bundle exec rails s`
- in another tab run `./bin/webpack-dev-server` (optional) 
- in another tab run `sidekiq` (optional, but necessary for things like password reset emails)
- navigate to `http://localhost:3000`

## Environment Variables
If you want functionality like password reset emails to work locally, you'll need to set the following environment variables in `config/application.yml` with your own unique values:
```
ROOT_URL: http://localhost:3000
SENDGRID_API_KEY: xxxxxxxxxxxxxx
SENDGRID_USERNAME: xxxxxxxxxxxxxx
SENDGRID_PASSWORD: xxxxxxxxxxxxxx
DEFAULT_FROM_EMAIL: you@example.com