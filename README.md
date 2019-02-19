# Minimal Ruby and NodeJS/NPM/Yarn built on top of Alpine Linux Docker Image (Approx. 53MB)
Self explanatory, ruby build on top of nodejs and alpine image

This will be a great base image for people working with rails applications.
You could get away from using therubyracer gem by using a pre-built nodejs for the javascript V8 engine.

Hope this will help others in the future.

### Tags and Versions
- [`2.1.9`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.1.9/Dockerfile)
- [`2.2.3`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.2.3/Dockerfile)
- [`2.2.4`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.2.4/Dockerfile)
- [`2.2.5`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.2.5/Dockerfile)
- [`2.2.6`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.2.6/Dockerfile)
- [`2.2.7`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.2.7/Dockerfile)
- [`2.2.8`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.2.8/Dockerfile)
- [`2.2.9`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.2.9/Dockerfile)
- [`2.2.10`, `2.2`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.2.10/Dockerfile)
- [`2.3.0`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.3.0/Dockerfile)
- [`2.3.1`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.3.1/Dockerfile)
- [`2.3.3`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.3.3/Dockerfile)
- [`2.3.4`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.3.4/Dockerfile)
- [`2.3.5`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.3.5/Dockerfile)
- [`2.3.6`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.3.6/Dockerfile)
- [`2.3.7`, `2.3`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.3.7/Dockerfile)
- [`2.4.1`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.4.1/Dockerfile)
- [`2.4.2`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.4.2/Dockerfile)
- [`2.4.4`, `2.4`, `latest`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.4.4/Dockerfile)
- [`2.5.0`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.5.0/Dockerfile)
- [`2.5.1`, `2.5`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.5.1/Dockerfile)
- [`2.6.1`, `2.6`](https://github.com/Daniel-ltw/ruby-node-alpine/blob/master/2.6.1/Dockerfile)


### Gem dependencies
When you install gems, there are gems with specific native dependencies.

You have to add the respective alpine package before installing the respective gems.
```
apk --update add ${packages}
```

The few known dependencies are:
* ffi: libffi-dev
* nokogiri: libxml2 libxslt libxml2-dev libxslt-dev
* rmagick: imagemagick imagemagick-dev
* raindrops: linux-headers
* pg: postgresql-client postgresql-dev

p.s.: there are also a few native compilation dependencies that you have to keep in mind.
* g++
* make


### Supported Docker versions

This image is officially supported on Docker version 1.11.2.

Support for older versions (down to 1.6) is provided on a best-effort basis.

### Contributing

You are invited to contribute new features, fixes, or updates, large or small.

I am always thrilled to receive pull requests, and do my best to process them as fast as I can.
