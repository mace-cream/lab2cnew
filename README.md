# How to maintain this website

This website is based on Hugo static site generator.
It is deployed to [lab2cnew](http://10.8.4.170/lab2cnew/).

## How to edit our team
Check directory `data/en/team.yml`, make sure your photo is 670X670 pixels.

## How to edit our research
Check directory `content/blog`, add new posts or edit existing posts.

## How to put pictures in our post

## How to check build error
On your commit to this repository, gitlab will automatically build the website source code. If the build is 
successful, the build artifact will be deployed to our manage node web directory. To check whether the build is successful and
the build log, you can
open the [pipelines](http://10.8.4.170:88/zhaofeng-shu33/lab2cnew/pipelines) web page.

## How to format our published article
First we should make a bibtex database. See the project [lab-bibtex](http://10.8.4.170:88/zhaofeng-shu33/lab-bibtex).
Then use `pybtex` to generate markdown file.
