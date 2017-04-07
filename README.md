# ACF

> An [Advanced Custom Fields](https://www.advancedcustomfields.com) helper for [WordPlate](https://wordplate.github.io).

```php
$fields = [
    acf_image(['name' => 'image', 'label' => 'Image']),
    acf_text(['name' => 'title', 'label' => 'Title']),
];

$location = [
    acf_location('post_type', 'post'),
    acf_location('post_type', '!=', 'page'),
];

acf_field_group([
    'title' => 'About',
    'key' => 'group_about',
    'fields' => $fields,
    'location' => [
        $location,
    ]
]);
```

[![Build Status](https://img.shields.io/travis/wordplate/acf/master.svg?style=flat)](https://travis-ci.org/wordplate/acf)
[![StyleCI](https://styleci.io/repos/87427318/shield?style=flat)](https://styleci.io/repos/87427318)
[![Coverage Status](https://img.shields.io/codecov/c/github/wordplate/acf.svg?style=flat)](https://codecov.io/github/wordplate/acf)
[![Latest Version](https://img.shields.io/github/release/wordplate/acf.svg?style=flat)](https://github.com/wordplate/acf/releases)
[![License](https://img.shields.io/packagist/l/wordplate/acf.svg?style=flat)](https://packagist.org/packages/wordplate/acf)

## Installation

Require this package, with [Composer](https://getcomposer.org/), in the root directory of your project.

```bash
$ composer require wordplate/acf
```

## License

[MIT](LICENSE) © [Vincent Klaiber](https://vinkla.com)
