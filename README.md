ErrorCollector
==============

Collector of latte exceptions for project build on [Nette Framework](http://nette.org).

## Installation
Easiest way is to use [Composer](http://getcomposer.org/):

```sh
$ composer require hotel-quickly/error-collector:@dev
```

## Usage

Mandatory configuration in config.neon
```yml
errorCollector:
	projectName: vanilla
	s3:
		accessKeyId:
		secretAccessKeyId:
		region: 'ap-southeast-1'
```

Full configuration list
```yml
errorCollector:
	s3:
		accessKeyId:
		secretAccessKeyId:
		region: 'ap-southeast-1'
		bucket: hq-error-log
	logDirectory: %appDir%/../log/
	errorStorage: '\HQ\Storage\S3Storage'
```

## The MIT License (MIT)

Copyright (c) 2014 Hotel Quickly Ltd.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
