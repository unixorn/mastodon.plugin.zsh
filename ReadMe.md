
# mastodon.plugin.zsh

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
![Awesomebot](https://github.com/unixorn/mastodon.plugin.zsh/actions/workflows/awesomebot.yml/badge.svg)
[![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2Funixorn%2Fmastodon.plugin.zsh%2Fbadge%3Fref%3Dmain&style=plastic)](https://actions-badge.atrox.dev/unixorn/mastodon.plugin.zsh/goto?ref=main)
![Megalinter](https://github.com/unixorn/mastodon.plugin.zsh/actions/workflows/mega-linter.yml/badge.svg)


<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
## Table of Contents

- [mastodon.plugin.zsh](#mastodon-toolszsh)
  - [Configuration](#configuration)
  - [Included Scripts](#included-scripts)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

Tools for interacting with mastodon from the command line.

## Configuration

Create a configuration file at `~/.mastodon-tools/preferences.sh` and set `FEDIVERSE_HOME` in it. the tools do no fancy parsing, they just source `preferences.sh` to find out what fediverse host is home for you.

```sh
FEDIVERSE_HOME='https://hachyderm.io'
```

## Included Scripts

| Script | Original Source | Description |
| ------ | --------------- | ----------- |
| `mastodon-last-post` | Here | Shows when the user last posted. Requires that their home server allows unauthenticated API read access. |
| `mastodon-summary` | Here | Prints a quick summary of a given mastodon user. Requires that their home server allows unauthenticated API read access. |
| `mastodon-user-profile` | Here | Uses macOS `open` command to open browser pages for the given fediverse users on your server so you can easily follow them. |
