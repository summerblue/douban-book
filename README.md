<h1 align="center"> douban-book </h1>

<p align="center"> :green_book: A book SDK.</p>

[![Build Status](https://travis-ci.org/Littlesqx/douban-book.svg?branch=master)](https://travis-ci.org/Littlesqx/douban-book)
[![StyleCI](https://github.styleci.io/repos/150088434/shield?branch=master)](https://github.styleci.io/repos/150088434)
## Installing

```shell
$ composer require littlesqx/douban-book -vvv
```

## Usage

```php
<?php

// init app
$app = new Littlesqx\Book\Application();

// book's isbn10/isbn13 code
$isbn = '9787115473899';

// get a book entity
$book = $app->getBook($isbn);

// use as an array
$book->toArray();

// or get json format
$book->toJSON();

// also, get property directly is allowed
$book->getTitle();
$book->getPrice();
```

## Contributing

You can contribute in one of three ways:

1. File bug reports using the [issue tracker](https://github.com/littlesqx/douban-book/issues).
2. Answer questions or fix bugs on the [issue tracker](https://github.com/littlesqx/douban-book/issues).
3. Contribute new features or update the wiki.

_The code contribution process is not very formal. You just need to make sure that you follow the PSR-0, PSR-1, and PSR-2 coding guidelines. Any new code contributions must be accompanied by unit tests where applicable._

## Thanks

- [豆瓣 API](https://developers.douban.com)

- [overtrue](https://github.com/overtrue)

## PHP 扩展包开发

> 想知道如何从零开始构建 PHP 扩展包？
>
> 请关注我的实战课程，我会在此课程中分享一些扩展开发经验 —— [《PHP 扩展包实战教程 - 从入门到发布》](https://learnku.com/courses/creating-package)

## License

MIT
