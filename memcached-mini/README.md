memcached-mini
===

This is a Docker image for [memcached](http://memcached.org/) running on
[Alpine Linux](http://alpinelinux.org/), a very tiny distribution.

Why?
---
This image lets you run memcached on Alpine Linux, a tiny distribution
based on Busybox. You get a full memcached installation in a much smaller
image and with a smaller footprint than those based on Ubuntu or other
full-fledged distribution.

The total image size of memcached-mini, including the operating system, is
only around 50 MB.

Build
---

    # docker build -t `whoami`/memcached-mini .

Usage
---
To run a memcached container and map the host's port 11211 to it, try:

    # docker run -d -p 11211:11211 `whoami`/memcached-mini

You can pass any extra arguments to memcached with `docker run. For
example, to see memcached help, just do:

    # docker run `whoami`/memcached-mini -h
    memcached 1.4.19
    -p <num>      TCP port number to listen on (default: 11211)
    -U <num>      UDP port number to listen on (default: 11211, 0 is off)
    -s <file>     UNIX socket path to listen on (disables network support)
    ...
