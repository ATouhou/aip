# Arabic in PHP (AIP)

[![Latest Stable Version](https://poser.pugx.org/buzzylab/aip/v/stable)](https://packagist.org/packages/buzzylab/aip)
[![Total Downloads](https://poser.pugx.org/buzzylab/aip/downloads)](https://packagist.org/packages/buzzylab/aip)
[![Latest Unstable Version](https://poser.pugx.org/buzzylab/aip/v/unstable)](https://packagist.org/packages/buzzylab/aip)
[![License](https://poser.pugx.org/buzzylab/aip/license)](https://packagist.org/packages/buzzylab/aip)
[![StyleCI](https://styleci.io/repos/58194820/shield)](https://styleci.io/repos/58194820)

A simple PHP API extension that's provide arabic tools for PHP . [https://github.com/buzzylab/aip](https://github.com/buzzylab/aip)

> Note: AIP package is a built on the great library [Ar-PHP](http://www.ar-php.org/) (v4.0.0) which is developed by [Khaled Al-Sham'aa](http://www.ar-php.org/about-php-arabic.html).


## Contents
- [Features](#features)
- [Installation](#installation)
- [Change log](#change-log)
- [Issues](#issues)
- [Contributing](#contributing)
- [Credits & inspirations](#credits--inspirations)
- [License](#license)

## Features
* [Arabic text auto summarization](https://github.com/buzzylab/aip/blob/master/docs/Summarize.md).
* [Advanced Arabic search (stem based)](https://github.com/buzzylab/aip/blob/master/docs/Query.md).
* [Render Arabic text (PDF, GD, SWF)](https://github.com/buzzylab/aip/blob/master/docs/Glyphs.md).
* [Present dates in Arabic or Hijri](https://github.com/buzzylab/aip/blob/master/docs/Date.md).
* [Convert Hijri date into Unix timestamp](https://github.com/buzzylab/aip/blob/master/docs/Date.md).
* [Parse Arabic textual datetime into timestamp](https://github.com/buzzylab/aip/blob/master/docs/Date.md).
* [Transliterate English words in Arabic](https://github.com/buzzylab/aip/blob/master/docs/Transliteration.md).
* [Transliterate Arabic words in English](https://github.com/buzzylab/aip/blob/master/docs/Transliteration.md).
* [Spell numbers in Arabic idiom](https://github.com/buzzylab/aip/blob/master/docs/Numbers.md).
* [Phonetically alike Arabic words](https://github.com/buzzylab/aip/blob/master/docs/Soundex.md).
* [Arabic character set converter](https://github.com/buzzylab/aip/blob/master/docs/Charset.md).
* [Arabic character set auto detection](https://github.com/buzzylab/aip/blob/master/docs/Charset.md).
* [Identify Arabic in multi language documents](https://github.com/buzzylab/aip/blob/master/docs/Identifier.md).
* [Identify names & places in Arabic text](https://github.com/buzzylab/aip/blob/master/docs/Identifier.md).
* [Guess gender of Arabic names](https://github.com/buzzylab/aip/blob/master/docs/Gender.md).
* [Convert keyboard language programmatically](https://github.com/buzzylab/aip/blob/master/docs/KeySwap.md).
* [Calculate the time of Muslim prayer](https://github.com/buzzylab/aip/blob/master/docs/Salat.md).
* [Compress string using Huffman-like coding](https://github.com/buzzylab/aip/blob/master/docs/Compress.md).
* [Standardize Arabic text](https://github.com/buzzylab/aip/blob/master/docs/Standard.md).
* [Arabic stemmer](https://github.com/buzzylab/aip/blob/master/docs/Stemmer.md).
* Arabic Cities List
* Informations about Arabic countries
* [Arabic text normalisation](https://github.com/buzzylab/aip/blob/master/docs/Normalise.md).
* [Translate English words into Hieroglyphics](https://github.com/buzzylab/aip/blob/master/docs/Hiero.md).
* [Translate English words into Phoenician](https://github.com/buzzylab/aip/blob/master/docs/Hiero.md).





## Installation
### With Composer

```
$ composer require buzzylab/aip
```

Or Add `"buzzylab/aip": "~1.0.*"` to `composer require` :

```json
{
    "require": {
        "buzzylab/aip": "~1.0.*"
    }
}
```

#### Native Integration

```php

<?php
require 'vendor/autoload.php';

use Buzzylab\Aip\Arabic;

$arabic = new Arabic();

```

#### Laravel Integration

After installing the package, open your [Laravel](https://laravel.com) config file located at `config/app.php` and add the following service provider to the `providers` array:

```php
Buzzylab\Aip\Laravel\AipServiceProvider::class
```

And add the following Facade to the `aliases` array

```php
'Arabic'  => Buzzylab\Aip\Laravel\Facades\AipFacade::class 

```

## Change log
Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Issues
For the list of all current and former/closed issues see the [github issue list](https://github.com/buzzylab/aip/issues).
If you find a problem, please follow the same link and create an new issue, I will look at it and get back to you ASAP.

## Contributing
I would be glad to accept your contributions if you want to participate and share. Just follow GitHub's guide on how
to [fork a repository](https://help.github.com/articles/fork-a-repo/). Clone your repository to your machine, make
your change then create a pull request after submitting your change to your repository.

## Credits & inspirations
It goes without saying that none of this could have been done without the great [arphp](http://www.ar-php.org/)
library, a big thank you goes out to [Khaled Al-Sham'aa](http://www.ar-php.org/about-php-arabic.html).



### License
The AIP is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT).
