# Code examples for [Building RESTful API With ReactPHP](https://leanpub.com/building-restful-api-with-reactphp) Book.

### Quick start

1. Run docker-compose: 

```bash
docker-compose up
```

2. Install Composer dependencies:

```bash
docker-compose exec php composer install
```

3. Execute migrations:

```bash
docker-compose exec php ./vendor/bin/doctrine-migrations migrate
```

4. Use [requests.http](dev/requests.http) to send requests.

For requests that require authentication you need to register a new user first. 
Send `POST http://localhost:8000/auth/signup` to create a new user. Then send
`POST http://localhost:8000/auth/signin` to log in with this new user.
