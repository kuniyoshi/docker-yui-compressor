NAME
====

docker-yui-compressor

SYNOPSIS
--------

``` bash
  $ sudo docker pull kuniyoshi/docker-yui-compressor
  $ bin/yui-compressor [options] [input file]
```

DESCRIPTION
-----------

This repository builds a container of yui-compressor.
And includes, wrapper script placed in `bin/yui-compressor`.

SPECIAL PATHS
-------------

### /tmp/docker/yui-compressor

This path passes between user and docker container.
The files that are options to pass to the yui-compressor,
are `rsync`ed into `/tmp/docker/yui-compressor`.

After yui-compressor works, docker container saves
these files to the `/tmp/docker/yui-compressor`.

TODO
----

- make front end script portable, i.e. Windows
