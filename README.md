box-yeoman
=========

A box for building yeoman based projects. (includes: grunt, bower, phantomjs, karma)

In order to use the box you need to:

Add the next wercker.yml to your yeoman project:

    box: asabaylus/box-yeoman
    build:
        steps:
            - wercker/npm-install
            - olger/yeoman-bower-install
            - wercker/grunt:
                tasks: build

for a simple build.
