# mvisonneau/docker-geminabox


[![PULLS](https://img.shields.io/docker/pulls/mvisonneau/geminabox.svg)](https://hub.docker.com/r/mvisonneau/geminabox)
[![BUILD](https://img.shields.io/travis/mvisonneau/docker-geminabox/master.svg)](https://travis-ci.org/mvisonneau/docker-geminabox)

This docker image allows you to run a geminabox process. It is a forked from [ahmet2mir](https://github.com/ahmet2mir/dockerfiles/tree/master/geminabox) version, refactored to use the ruby alpine base image.

## Usage

```
docker run -d -p 9292:9292 --name geminabox mvisonneau/geminabox
```

If you want user based authentication:

```
docker run -d -p 9292:9292 -P -h geminabox --name geminabox -e USERNAME=user -e PASSWORD=password mvisonneau/geminabox
```

You can then access the app at the following URL http://localhost:9292
