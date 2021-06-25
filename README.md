# Neos Marker.io Package

[![Version](https://poser.pugx.org/muensmedia/neos-markerio/v/stable)](https://packagist.org/packages/muensmedia/neos-markerio)
[![license](https://poser.pugx.org/muensmedia/neos-markerio/license)](https://packagist.org/packages/muensmedia/neos-markerio)

## Introduction
**Collect website feedback from clients and colleagues on your Neos site using [Marker.io](https://marker.io/).**

This package integrates the `Marker.io` javascript snippet into Neos.

## Features
* adds Marker.io javascript snippet before the closing body tag
* configure the Marker.io destination
* show Marker.io only to authenticated users (e.g. after website launch)

## Installation

Run this in your site package

```console
composer require --no-update muensmedia/neos-markerio
```

Then run `composer update` in your project directory.

## Configuration

You can override the default configuration:

```yaml
Muensmedia:
  Neos:
    Markerio:
      destination: '606450c0bc25e5200845587f'
      displayOnlyForAuthenticatedUsers: true
```

### Activate Marker.io for all users
If your website is still in development, and you want to show Marker.io to all users (even unauthenticated users) you can set:
```yaml
Muensmedia:
  Neos:
    Markerio:
      displayOnlyForAuthenticatedUsers: false
```
## Contributions
Contributions are very welcome!

Please create detailed issues and PRs.

## License

See [License](./LICENSE)