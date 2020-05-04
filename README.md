# phpstan-craftcms

[![Latest Version on Packagist][ico-version]][link-packagist]
[![Software License][ico-license]](LICENSE.md)
[![Total Downloads][ico-downloads]][link-downloads]

Extension for PHPStan for better support for Craft CMS. The following features are provided:

- Configure autoload of Craft CMS for analysis
- Stub to support different `ElementQuery`-classes

## Install

Via Composer

``` bash
$ composer require --dev studio-stomp/phpstan-craftcms
```

## Usage

Add `phpstan-craftcms` to the project `phpstan.neon`:
```neon
includes:
    - vendor/studio-stomp/phpstan-craftcms/phpstan.neon
```

Feel free to check out the base configuration and expand on it with own configuration. For example:

```neon
includes:
    - vendor/studio-stomp/phpstan-craftcms/phpstan.neon

parameters:

    level: 2

    ignoreErrors:
        - '#Call to an undefined method SoapClient::#'
```

## Change log

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) and [CODE_OF_CONDUCT](CODE_OF_CONDUCT.md) for details.

## Security

If you discover any security related issues, please email hello@studiostomp.nl instead of using the issue tracker.

## Credits

- [Studio Stomp][link-author]
- [All Contributors][link-contributors]

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

[ico-version]: https://img.shields.io/packagist/v/studio-stomp/phpstan-craftcms.svg?style=flat-square
[ico-license]: https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square
[ico-travis]: https://img.shields.io/travis/studio-stomp/phpstan-craftcms/master.svg?style=flat-square
[ico-scrutinizer]: https://img.shields.io/scrutinizer/coverage/g/studio-stomp/phpstan-craftcms.svg?style=flat-square
[ico-code-quality]: https://img.shields.io/scrutinizer/g/studio-stomp/phpstan-craftcms.svg?style=flat-square
[ico-downloads]: https://img.shields.io/packagist/dt/studio-stomp/phpstan-craftcms.svg?style=flat-square

[link-packagist]: https://packagist.org/packages/studio-stomp/phpstan-craftcms
[link-downloads]: https://packagist.org/packages/studio-stomp/phpstan-craftcms
[link-author]: https://github.com/studio-stomp
[link-contributors]: ../../contributors
