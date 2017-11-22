<!-- -*- mode: markdown -*- coding: utf-8 -*- -->
# README

## Overview

* With site-generator "lektor" generate output into "docs" directory not "build"
* No use deploy method of lekter provided, use github commit/push only

## Set Up

create a project

    $ lecktor quickstart

* Project Name: blog-lektor
* Author Name: higebobo
* Project Path: [...]/blog-lektor (default)

## Github

create " blog-lektor" repository in github
    
## Deploy

initialize blog-lektor repository

    $ cd blog-lektor
    $ echo "*~" >> .gitignore
    $ echo "*.bak" >> .gitignore
    $ echo "*.pyc" >> .gitignore
    $ mv blog-lecktor.lektorproject website.lektorproject
    $ lektor build --output-path=docs
    $ git init
    $ git add .
    $ git commit -m 'First commit'
    $ git remote add origin git@github.com:higebobo/blog-lektor.git
    $ git remote -v
    $ git push -u origin master
    
set github pages master/docs

## Misc

### Plugin

* lektor-embed-x: embed youtube and twitter <sup id="a1">[1](#f1)</sup>

        $ lektor plugins add lektor-embed-x

## Footnotes

* <b id="f1">1:</b> iframe in github pages isn't allowed
