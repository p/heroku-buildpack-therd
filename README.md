This is an amalgamation of nodejs and php buildpacks:

- https://github.com/heroku/heroku-buildpack-nodejs
- https://github.com/heroku/heroku-buildpack-php

Having php work requires setting LD_LIBRARY_PATH in environment as follows:

heroku config:set LD_LIBRARY_PATH=/app/php/ext
