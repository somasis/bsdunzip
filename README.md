# bsdunzip, libarchive(1) unzip(1) from FreeBSD

[v3.7.0]: https://github.com/libarchive/libarchive/releases/tag/v3.7.0

> In 2023, libarchive (in [v3.7.0]) released their own port of FreeBSD's unzip,
> and it is now included in the base distribution. It is recommended that you
> use their port instead; this repository is now archived.

A [BSD-licensed](LICENSE) implementation of unzip(1), utilizing libarchive(1) as
the backend for interaction with the ZIP format. It is imported from the
[FreeBSD tree](https://github.com/freebsd/freebsd), with minor tweaks to make it
work on Linux (only two lines changed).

It is designed to provide an interface compatible with Info-ZIP's
[unzip(1)](http://www.info-zip.org/UnZip.html).

Currently synced with FreeBSD upstream as of [20160115].

## Requirements
- [libarchive](https://github.com/libarchive/libarchive)

## Installation
**Exherbo users, there is an exheres in ::somasis; app-arch/bsdunzip.**

1. `git clone https://github.com/Somasis/bsdunzip` or [download a release] [1].
2. `make`
3. `make install`

## Usage
After installation, you can read the manpage with `man bsdunzip`. A brief
listing of options and arguments is listed if you run `bsdunzip` with nothing as
arguments.

[20160115]: https://github.com/freebsd/freebsd/commit/4a483c2c396fcf156e04e080cce09e28143f5073
