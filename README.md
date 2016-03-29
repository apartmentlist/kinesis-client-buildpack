## `kinesis-client-buildpack` for Heroku

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) that
pulls in JAR files used to make use the Amazon [Kinesis Client Library][1].

[1]: http://docs.aws.amazon.com/kinesis/latest/dev/developing-consumers-with-kcl.html
g
It is meant to be used in conjunction with other buildpacks as part of a
[multi-buildpack](https://github.com/ddollar/heroku-buildpack-multi).

## Usage

Example usage:

    $ heroku buildpacks:set https://github.com/apartmentlist/kinesis-client-buildpack.git

    $ cat .buildpacks
    https://github.com/apartmentlist/kinesis-client-buildpack#1.0
    https://github.com/heroku/heroku-buildpack-ruby.git#v129


Don't forget to pin buildpack versions you want to use in your .buildpacks file.
