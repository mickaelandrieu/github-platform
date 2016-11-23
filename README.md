# PrestonBot

This application is based on Symfony CarsonBot and aims to help PrestaShop maintainers and contributors.

![Preston, the PrestaShop contributor best friend](http://i.imgur.com/r26gJW4.png)

## How to install ?

First of all you have to configure your GitHub repository and have a GitHub token.

```bash
composer install // and complete the interactive fields asked
```

## How to test ?

```bash
./vendor/bin/phpunit
```

You need also to create your own GitHub [personal token](https://github.com/settings/tokens) and export it:

```bash
export GH_TOKEN=XXXXXXXXXXXXXXXXXXXXXXXXXXXX
```

## Our standards ?

Yeah, mostly the *Symfony* ones:

```bash
./vendor/bin/php-cs-fixer fix . # we use the Symfony level + short array notation filter
```

## What is Preston capable of doing?

* Check a pull request description according to *PrestaShop* standards;
* Check pull request commits labels according to *PrestaShop* standards;
* Extract data from the pull request and look for some terms;
* Welcome every new contributor;
* Manage labels;
