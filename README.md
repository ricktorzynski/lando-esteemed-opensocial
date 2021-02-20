# Open Social Local Dev Using Lando

This repo is set up to be used in setting up a local dev environment using [Lando](https://lando.dev/).

## Prerequisites

1. [Composer](https://getcomposer.org/download/) installed locally.
2. [Lando](https://lando.dev/) installed locally.

## Installation of Open Social for Lando

```
$ git clone https://github.com/ricktorzynski/lando-esteemed-opensocial
$ cd lando-esteemed-opensocial
$ composer install
$ lando init
```
For the install and note the root directory is "html" and not "web"
```
From where should we get your app's codebase? current working directory
What recipe do you want to use? drupal8
Where is your webroot relative to the init destination? html
What do you want to call this app? esteemed-open-social
```
Start Lando up to create docker containers
```
$ lando start
```
Boomshakalaka!!!
You will be shown the site url:
```
 NAME            esteemed-open-social                        
 LOCATION        /home/rick/Lando/esteemed-opensocial        
 SERVICES        appserver, database                         
 APPSERVER URLS  https://localhost:32775                     
                 http://localhost:32776                      
                 http://esteemed-open-social.lndo.site:8000/ 
                 https://esteemed-open-social.lndo.site/    
```
Go to the URL in your browser and commence the install.


### Install issues for Open Social
[documentation](https://www.drupal.org/docs/8/distributions/open-social/installing-and-updating)

### Installing outside of HTML folder
[See this issue for more information](https://www.drupal.org/project/social/issues/2792543#comment-11591981)


