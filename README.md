# Lighthouse Paperclip

[![Latest Version on Packagist](https://img.shields.io/packagist/v/daniel-de-wit/lighthouse-paperclip.svg?style=flat-square)](https://packagist.org/packages/daniel-de-wit/lighthouse-paperclip)
[![Build Status](https://img.shields.io/travis/daniel-de-wit/lighthouse-paperclip/master.svg?style=flat-square)](https://travis-ci.org/daniel-de-wit/lighthouse-paperclip)
[![Quality Score](https://img.shields.io/scrutinizer/g/daniel-de-wit/lighthouse-paperclip.svg?style=flat-square)](https://scrutinizer-ci.com/g/daniel-de-wit/lighthouse-paperclip)
[![Total Downloads](https://img.shields.io/packagist/dt/daniel-de-wit/lighthouse-paperclip.svg?style=flat-square)](https://packagist.org/packages/daniel-de-wit/lighthouse-paperclip)

This package will add two directives that will support working with [czim/laravel-paperclip](https://github.com/czim/laravel-paperclip).

![](lighthouse-paperclip-demo.gif)

## Installation

You can install the package via composer:

```bash
composer require daniel-de-wit/lighthouse-paperclip
```

## Usage

Apply the `@attachment` directive to get an url for the attachment.
``` graphql
type Blog {
    image: String @attachment
}
```

Apply the `@variant` to automatically generate an enum for available variant resizes. 
``` graphql
type Blog {
    image(variant: _ @variant): String @attachment
}
```

### Testing

``` bash
composer test
```

### Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Credits

- [Daniel de Wit](https://github.com/daniel-de-wit)
- [All Contributors](../../contributors)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
