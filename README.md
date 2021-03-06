# Instagram Challenge

## The Mission
Build Instagram using Rails. 

## How to Set-up

Clone this repo and navigate to the directory: 
```
git clone https://github.com/EsamAl-Dabagh/instagram-challenge.git
cd instagram-challenge
```

Install all the relevant dependencies:
`bundle install`

Set-up the database:
`rake db:drop db:create db:migrate db:seed`

## How to Use

`rails server`

Then navigate to `http://localhost:3000/` in your browser.

##### Browse a timeline of posts:
![Imgur](https://i.imgur.com/QpyAbyC.png)

##### Click on an author of a post to see all posts by that author:
![Imgur](https://i.imgur.com/SlGdE0y.png)

##### User can sign-up:
![Imgur](https://i.imgur.com/V4np6Y9.png)

##### A previously registered user can login:
![Imgur](https://i.imgur.com/sKdzYCN.png)

## User Stories

```
As a user
So that I can use the service
I want to be able to sign up
```
```
As a user
So that I can share my images
I want to be able to post a picture
```
```
As a user
So that I can keep up-to-date
I want to be see pictures in reverse chronological order
```
```
As a user
So that I can quickly give kudos for a picture
I want to be able to like a picture
```

## Domain Model
```
                   ╔═════════════════╗
                   ║   CONTROLLERS   ║
╔════════╗         ║                 ║          ╔═══════╗
║ Routes ║ ------> ║     Users       ║ -------> ║ Views ║
╚════════╝         ║     Posts       ║          ╚═══════╝
                   ║     Likes       ║
                   ╚═════════════════╝
                            |
                            |
                      ╔════════════╗
                      ║   MODELS   ║
                      ║            ║
                      ║   User     ║
                      ║   Post     ║
                      ║   Like     ║
                      ╚════════════╝
```

## Testing
Run tests from the command line using `rspec`. 
* TDD'd using RSpec and Capybara.
* Coverage = 100% (provided by SimpleCov)

![Imgur](https://i.imgur.com/HxkKE1U.png)