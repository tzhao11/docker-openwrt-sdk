# docker-openwrt-sdk

[![License: MIT](http://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://github.com/hnw/docker-openwrt-sdk/blob/master/LICENSE)


This is a docker container for the [OpenWRT](https://openwrt.org/) SDK.

```sh
$ docker run -it -v "$(pwd)/bin:/sek/bin/" aparcar/openwrt-sdk:18.06-ar71xx /bin/bash
```

Then you can build packages as follows:

```sh
# ./scripts/feeds update -a
# ./scripts/feeds install htop
# make package/htop/compile V=s
```

More information on how to use the SDK tool-chain can be found in the
[OpenWRT documentation](https://openwrt.org/docs/guide-developer/using_the_sdk).
