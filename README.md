# nodejs-bower-gulp

This Dockerfile extends `debian:wheezy` and installs node, bower, gulp, sass, compass, and libraries that are required for some builds. It is intended to be used for building the assets in your project.

The workdir is set to `/app`.

# Example uses

```
docker run --rm -v `pwd`:/app evolution7/nodejs-bower-gulp npm install
docker run --rm -v `pwd`:/app evolution7/nodejs-bower-gulp bower install
docker run --rm -v `pwd`:/app evolution7/nodejs-bower-gulp gulp build
```
