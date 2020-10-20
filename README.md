# CuboEducativo Raspbian Image

[![Build Status][gh-actions]][actions]
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

[gh-actions]: https://action-badges.now.sh/CuboEducativo/image?action=build
[actions]: https://github.com/CuboEducativo/image/actions

This repository allows you to build CuboEducativo Raspbian image using [packer-builder-arm's](https://github.com/mkaczanowski/packer-builder-arm) [docker](https://www.docker.com/get-started) image

# Quick start

Note: this assumes you already have docker installed locally.

```
git clone https://github.com/CuboEducativo/image
cd image
docker run --rm --privileged -v /dev:/dev -v ${PWD}:/build mkaczanowski/packer-builder-arm build raspbian.json
```

# What's inside

So far it's preconfigured with:

-   [Box86](https://github.com/ptitSeb/box86)
-   [Zoom](https://zoom.us/) (thanks to [Box86](https://github.com/ptitSeb/box86/issues/193))
