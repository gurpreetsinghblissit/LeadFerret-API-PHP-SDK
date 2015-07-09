[![Build Status](https://travis-ci.org/leadferret/LeadFerret-API-PHP-SDK.svg)](https://travis-ci.org/leadferret/LeadFerret-API-PHP-SDK)

# LeadFerret-API-PHP-SDK

## Description

Client SDK for the LeadFerret API - written in PHP. Allows you to work with the LeadFerret End-User API. 

## Installation 

For now just check out the repo from git. Later we will add it to packagyst so you can composify it.  

    `git clone https://github.com/leadferret/LeadFerret-API-PHP-SDK.git`

## Beta ##

This library is in Beta. Contact us if you wish to have more details. 


## Usage

Make sure you set up your .env file properly.  This client uses [DotEnv](https://github.com/vlucas/phpdotenv) to handle the environment and config items. 

This distribution comes with an example config `.env.example` and inside this file are some of the environment variables that should be used to set up the application. 

## Requirements ##
* [PHP 5.5.1 or higher](http://www.php.net/)
* [PHP JSON extension](http://php.net/manual/en/book.json.php)


## Developer Documentation ##

Please note documentation found at [apiary.io](http://docs.leadferretuser.apiary.io/#)

## Basic Example ##

See the examples/ directory for examples of the key client features.
```PHP
<?php

include_once '../bootstrap.php';
use LeadFerret\LFClient;

$client = new LFClient();
$token = $client->authenticate();

echo $token;
  
```
