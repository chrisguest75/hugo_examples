# README.md
Hugo examples with themes.  

This repository contains a playground where I'm playing with a few hugo themes.  

## TODO:
* Instructions for linux.
* Build public folder and commit into a pages repo
* CNAME example.  
* submodules instructions 
* TIL - learned
* food blog


## Installation
```sh
# extended version is installed by default on mac.
brew install hugo

# init the submodules

```

## Creating an example
Following the [quickstart](https://gohugo.io/getting-started/quick-start/) using [themes](https://themes.gohugo.io/) from the list.   
```sh
#  
hugo new site quickstart

git submodule add https://github.com/jakewies/hugo-theme-codex.git themes/hugo-theme-codex

hugo new posts/my-first-post.md         
hugo server -D

```


```sh
# build the final render in public directory 
hugo -D
```

## quickstart 
https://themes.gohugo.io/themes/hugo-theme-codex/


## loveit 
https://themes.gohugo.io/themes/loveit/

