# A slightly more opinionated version of Spatie's Laravel Stubs package.

This repo contains opinionated versions of the Laravel stubs. The most notable changes are:

- migrations don't have a `down` function
- controllers don't extend a base controller
- none of the model attributes are guarded
- use return type hints where possible
- most docblocks have been removed
- Added `declare(strict_types=1);` to all stubs

## Installation

You can install the package via composer:

```bash
composer require thepublicgood/laravel-stubs --dev
```

If you want to keep your stubs up to date with every update, add this composer hook to your composer.json file:

```json
"scripts": {
    "post-update-cmd": [
        "@php artisan tpg-stub:publish --force"
    ]
}
```

## Usage

You can publish the stubs using this command:

```bash
php artisan tpg-stub:publish
```

## Testing

``` bash
composer test
```

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information on what has changed recently.

## Contributing

Please see [CONTRIBUTING](https://github.com/spatie/.github/blob/main/CONTRIBUTING.md) for details.

## Security

If you've found a bug regarding security please mail [makers@thepublicgood.dev](mailto:makers@thepublicgood.dev) instead of using the issue tracker.

## Credits

- [Freek Van der Herten](https://github.com/freekmurze)
- [All Contributors](../../contributors)
- [Warrick Bayman](https://github.com/warrickbayman)

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
