APPRENTISSAGE DE REACT_JS

## Setup


```
composer install
```


**Setup the Database**

Open `.env` and make sure the `DATABASE_URL` setting is
correct for your system.

Then, create the database and the schema!

```
php bin/console doctrine:database:create
php bin/console doctrine:migrations:migrate
php bin/console doctrine:fixtures:load
```

**Build your Assets**

To build your assets, install the dependencies with yarn and then
run encore:

```
yarn install
yarn run encore dev --watch
```

**Start the built-in web server**

You can use Nginx or Apache, but the built-in web server works
great:

```
php bin/console server:run
```

Now check out the site at `http://localhost:8000`
