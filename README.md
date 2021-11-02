# README.md
Hugo examples with themes.  

This repository contains a playground where I'm playing with a few hugo themes.  

## TODO:
* Instructions for linux.
* Build public folder and commit into a pages repo
* submodules instructions 
* TIL - learned
* food blog
* Can I embed a 3d spinning globe onto my hugo about page?  

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
hugo new blog/my-first-blog.md         
hugo server -D
```

```sh
# create ico file
magick -density 128x128 -background none ./resources/me.png -resize 128x128 ./resources/favicon.ico
```

## quickstart 
Using the [hugo-theme-codex](https://themes.gohugo.io/themes/hugo-theme-codex/) theme. 

Demonstrates examples of using emojis and linking images into the posts.  
```ini
enableEmoji = true
```

```sh
# build the final render in public directory 
cd quickstart
hugo -D
```


## loveit 
https://themes.gohugo.io/themes/loveit/


# Resources
* A walkthrough from [freecodecamp](https://www.freecodecamp.org/news/your-first-hugo-blog-a-practical-guide/)
* awesome-hugo https://github.com/theNewDynamic/awesome-hugo