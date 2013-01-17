## Travis CI ember web client

### Running the app

In order to run the app you need to install dependencies with:

    bundle install

Then you have to run the server, the easiest way to do this is to
use foreman:

    bundle exec foreman start

Now you can open [localhost:5000](http://localhost:5000)

By default it uses official API at `https://api.travis-ci.org`, but you
can set your own enpoint using:


    API_ENDPOINT="http://localhost:300/" bundle exec foreman start

This will run against API run locally.

### Compiling assets manually

    bundle exec rakep
    ENV=production bundle exec rakep
