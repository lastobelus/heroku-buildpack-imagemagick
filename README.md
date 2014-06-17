heroku-buildpack-imagemagick
===========================

Use the latest version of ImageMagick inside Heroku _Cedar_.
At the moment it is bundled the version **6.8.0-3.**

* libpng-1.6.12
* libjpeg-turbo-1.3.1


## Usage

This buildpack is built to be used through 
[heroku-buildpack-multi](https://github.com/ddollar/heroku-buildpack-multi),
so in your app you need to:
```
heroku config:set BUILDPACK_URL=https://github.com/ddollar/heroku-buildpack-multi
```

Then, create a `.buildpacks` file inside your app:
```
https://github.com/pepabo/heroku-buildpack-imagemagick
https://github.com/heroku/heroku-buildpack-nodejs
```

This example was based on the nodejs buildpack, but it can be used with
any other.
If it is not working with yours, please report a bug.
