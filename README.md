Heroku Buildpack: Jpegoptim
=======================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for using [jpegoptim](https://github.com/tjko/jpegoptim) in your application.

It is designed to be used with [heroku-buildpack-multi](https://github.com/ddollar/heroku-buildpack-multi) to combine it with the appropriate real buildpack for your app.

Or even heroku added built-in [multi buildpack support](https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app) .

Usage
-----
Add a `.buildpacks` file to the root of your repo that contains this buildpack URL and your real buildpack URL:

    https://github.com/yagainc/heroku-buildpack-jpegoptim
    https://github.com/heroku/heroku-buildpack-ruby

Or

    heroku buildpacks:add https://github.com/yagainc/heroku-buildpack-jpegoptim

You can verify that everything is properly installed by running the following command:

    $ heroku run "jpegoptim -V"

