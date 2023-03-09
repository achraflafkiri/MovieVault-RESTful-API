
# MovieValut RESTful API

The app is a RESTful API built using Node.js.
The main functionality of the app is to manage a collection of music files, which users can create, read, update, and delete (CRUD operations) through the API endpoints.
The app also provides user authentication and authorization through a login and signup feature, where users can create an account and login to access the protected API endpoints.
The app allows users to share music files with their friends through the API endpoints.
The app is named "MovieVault-RESTful-API", which suggests that it may also have a feature for managing and storing movie files, although this is not mentioned in the provided description.

    

## Installation

Clone the project

```bash
  git clone https://github.com/achraflafkiri/restful-movie-app.git
```

Go to the project directory

```bash
  cd restful-movie-app
```

Install dependencies

```bash
  npm install
```

Configure `.env` file with this variables :
- `PORT` -> localhost port
- `DB_URL` -> your mongo db url
- `SECRET_KEY` -> the key that the JWT will use

Start the server

```bash
  npm run start
```


## Requests

AUTH
```bash
/api/v1/auth/register   [POST]
/api/v1/auth/login      [POST]
```

USERS
```bash
/api/v1/users        [GET]
/api/v1/users/:id    [GET]
/api/v1/users/:id    [PATCH]
/api/v1/users/:id    [DELETE]
```

MOVIES
```bash
/api/v1/movies        [GET]
/api/v1/movies        [POST]
/api/v1/movies/:id    [GET]
/api/v1/movies/:id    [PATCH]
/api/v1/movies/:id    [DELETE]
```

LISTS
```bash
/api/v1/lists        [GET]
/api/v1/lists        [POST]
/api/v1/lists/:id    [DELETE]
```




## Queries


USERS
```bash
/api/v1/users/?limit=10  [GET]
```

MOVIES
```bash
/api/v1/movies/?genre=romantic  [GET]
/api/v1/movies/?type=serie      [GET]

```

LISTS
```bash
/api/v1/lists/?genre=romantic  [GET]
/api/v1/lists/?type=serie      [GET]
``` 




