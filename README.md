# RESTful API Authentication With JWT (TDD Approach)

This is a tutorial course. In this project, we set up a simple Rails API-only-application. Rails API-only-applications are slimmed down compared to traditional Rails web applications. we we'll secure the login, register, and our book's endpoint using JWT.

## Built With

- Ruby v2.7.2
- Ruby on Rails v6.0.3.2
- RSpec-Rails for testing


## Current API Endpoints

The API will expose the following RESTful endpoints.
### BaseUrl: {Host-URL}/api/v1

| Endpoint                | Functionality                |
|-------------------------|------------------------------|
| POST /register          | Signup                       |
| POST /login             | Login                        |
| GET /books              | Get all books                |
| GET /books/:id          | Get a bppl                   |
| POST /books             | Add a new book               |
| DELETE /books/:id       | Delete a book                |
| PUT /books/:id          | Update a book                |
| POST /categories        | Add category                 |
| GET /categories         | Get categories               |


To get a local copy up and running follow these simple example steps.

### Prerequisites

Ruby: 2.6.5
Rails: 6.0.3.2
Postgres: >=9.5

### Setup

~~~bash
$ git clone https://github.com/Oxford-G/books-api.git
$ cd books-api
~~~

Install gems with:

```
bundle install
```

Setup database with:

> make sure you have postgress sql installed and running on your system

```
   rails db:create
   rails db:migrate
   rails db:seed
```

### Usage

Start server with:

```
    rails server
```

Open `http://localhost:3000/` in your browser.

### Deploy to a live server

Deploying to a live server like Heroku is easy, make sure you have the necessary credentials setup on your local machine

```bash
heroku create
heroku rename app-new-name
git push heroku $BRANCH_NAME:master 
```
if you are already in master branch no need to add $BRANCH_NAME, just use `git push heroku master`

```bash
heroku run rails db:migrate
heroku run rails db:seed
heroku open
```

Enjoy your newly deployed rails API


### Run tests

```
    rpsec 
```

# Authors

👤 **Enekwechi Chinonso Gerald**

- GitHub: [@Oxford-G](https://github.com/Oxford-G)
- Twitter: [@OXFORD2](https://twitter.com/OXFOXD2)
- Linkedin: [Enekwechi Chinonso G](https://www.linkedin.com/in/chinonso-enekwechi)


## 🤝 Contributing

Contributions, issues and feature requests are welcome!

Feel free to check the [issues page](issues/).

## Show your support

Give a ⭐️ if you like this project!

