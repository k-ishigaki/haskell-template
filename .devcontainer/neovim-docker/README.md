# neovim-docker

A nvim excutable via Docker.
Alpine base image, includes vim-plug, coc.nvim, etc.

## Features

 * Changeable uid/gid when running container
 * Plugins embedded (using vim-plug)
 * Language Server Protocol Support (using coc.nvim)

## Requirements

 * Docker

## Run

```Shell
docker run --rm -it -v $(pwd):/root/workspace -w /root/workspace -u $(id -u):$(id -g) ghcr.io/k-ishigaki/neovim-docker nvim ...
```
