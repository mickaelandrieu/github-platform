# Community Platform

Community Platform gives you an easy api and tools to make your own Github bots and tools.

## How to install ?

You need to create your own GitHub [personal token](https://github.com/settings/tokens).
After installation and the hosting of your community-platform project, you need to register a [webhook](https://developer.github.com/webhooks/creating/#setting-up-a-webhook) to get
information from GitHub.

Then, you must configure a [Secured GitHub token](https://developer.github.com/webhooks/securing/#setting-your-secret-token).

### Classic installation

First of all you have to configure your GitHub repository and have a GitHub token.

```bash
composer install // and complete the interactive fields asked
```

### Docker installation

First, setup the `docker-compose.yml` file with a valid GitHub token and a valid Secure token (can be empty).

```bash
make start
```

The Home page is now available at "http://localhost:81/".

## How to test ?

```bash
./vendor/bin/simple-phpunit
# or (using docker)
make test
```

> To launch tests suite, you only need to setup your own Github token (`GH_TOKEN`).

## Our standards ?

Yeah, mostly the *Symfony* ones:

```bash
./vendor/bin/php-cs-fixer fix # we use the Symfony level + short array notation filter
```

## What can I expect from the Community Platform?

* Comment on a pull request to help a contributor fix his work;
* Extract data from the pull request and look for some terms;
* Manage labels;
* Validate a pull request description;
* Welcome every new contributor;
* Labelize a PR regarding information in description
* Labelize a PR regarding files updated
