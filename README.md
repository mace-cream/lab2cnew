# Lab2c Website

## How to maintain this website

This website is based on Hugo static site generator.
It is deployed to [lab2cnew](http://10.8.4.170/lab2cnew/) for intranet
and [mace-cream](https://mace-cream.github.io/) for outside access.

## How to edit our team
Check directory `data/en/team.yml`, make sure your photo is 670X670 pixels.

## How to edit our research
Check directory `content/blog`, add new posts or edit existing posts.

## How to put pictures in our post
Put your pictures in `static/images/blog`.

## How to create new research articles
Check `content/research`; Copy a file from `research-article-template.md` and change it to your custom names; Change the contents of your md file and you are done.

How to add new menu entry

First create a new directory called A in `content` (copied from others in the same directory). And then create another directory A in `themes/navigator-hugo/layouts`(copied from others in the same directory). Finally create a file `A.html` in `themes/navigator-hugo/layouts`.

## How to check build error
On your commit to this repository, gitlab will automatically build the website source code. If the build is 
successful, the build artifact will be deployed to our manage node web directory. To check whether the build is successful and
the build log, you can
open the [pipelines](http://10.8.4.170:88/zhaofeng-shu33/lab2cnew/pipelines) web page.

## How to format our published article
First we should make a bibtex database. See the project [lab-bibtex](http://10.8.4.170:88/zhaofeng-shu33/lab-bibtex).
Then use `pybtex` to generate markdown file.

## About CICD of this project
Use docker to start the `gitlab-runner` service
```shell
docker-compose start
```
## Local Development
Install [hugo](https://gohugo.io/getting-started/installing/).
Build by `hugo -b http://127.0.0.1:8000`. You can not build by other ip addresses since
the BaiduMap API is bound with `*.github.io,10.8.4.170,127.0.0.1`.

## Push to Github
Since the master branch is reserved for publication, you should use `dev` branch to push to github.
```shell
git checkout dev
git merge master
git push github dev
git checkout master
```

## How to compress video
```shell
ffmpeg -i input.mp4 -s 960x540 -c:a copy output.mp4
```