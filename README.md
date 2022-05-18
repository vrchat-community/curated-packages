# VRChat Curated Packages

# About
This repository hosts a listing for a curated list of helpful and safe packages to use in your VRChat project.

It is designed for use with the [Creator Companion](https://vcc.docs.vrchat.com/).

You can also use this repo as a template to make your own package listing if you'd like. More on that later.

## How it works

We store a very simple list of urls in [list.yml](list.yml). 

Each url points to a publicly-accessible [VPM-compatible manifest file](https://vcc.docs.vrchat.com/vpm/packages#package-format).


When this file is changed, a GitHub Action runs which fetches each manifest and combines them into a JSON object in the [Repo List format](https://vcc.docs.vrchat.com/vpm/repos#format).

This new [index.json](docs/index.json) file is then committed to `docs/index.json`, where GitHub Pages will serve it up as a public file!
