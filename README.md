# VRChat Curated Packages

{% note %}

**DON'T USE THIS YET!**

This repo is public in order to serve [a repo listing endpoint](https://vrchat-community.github.io/curated-packages/) for a closed beta test. You may not be able to access the content to which it points until this project goes to Open Beta.

{% endnote %}

This repository hosts a listing for a curated list of helpful and safe packages to use in your VRChat project.

It is designed for use with the [Creator Companion](https://docs.vrchat.com/docs/creator-companion-overview).

You can also use this repo as a template to make your own package listing if you'd like. More on that later.

## How it works

We store a very simple list of urls in [list.yml](list.yml). 

Each url points to a publicly-accessible [VPM-compatible manifest file](https://docs.vrchat.com/docs/packages#package-format).


When this file is changed, a GitHub Action runs which fetches each manifest and combines them into a JSON object in the [Repo List format](https://docs.vrchat.com/docs/repos#format).

This new [index.json](docs/index.json) file is then committed to `docs/index.json`, where GitHub Pages will serve it up as a public file!
