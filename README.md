# debian-mirror

This is a Docker container for a debian mirror

## Requirements

* Docker
* .deb files you want to use to create a mirror

## Installation

* `docker run -d brimstone/debian-mirror`

## Usage

* `rsync` over any debs you want into the `pool` endpoint, sorted by distro. Everything else is automagic.

## Pool Directory structure

`pool` This is the main pool directory.

`+-> trusty` This is the directory for Ubuntu Trusty specific files.

`+-> trusty -> chef` This is for custom builds of chef for trusty.

`+-> sid` This is for Debian Sid specific packages.