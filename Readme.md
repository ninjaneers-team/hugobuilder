# README
(c) Ninjaneers GmbH 2016

## Preface
This Dockerfile will provide the static page generator hugo.
It is inspired by publysher/hugo.
In contrast to most other hugo Dockerfiles this one is intended to only render the target files.

## Usage
The following will let the container run from the current workdir and write into the local directory target.
By default the destination directory will be cleaned!

    docker run --rm -ti --volume=`pwd`:/source --volume=`pwd`/target:/target ninjaneers/hugobuilder

