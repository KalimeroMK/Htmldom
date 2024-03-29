Htmldom
=======

A Htmldom package for Laravel 5 to 9 based on Simple HTML Dom Parser

## Installation

Add the following line to the `require` section of `composer.json`:

composer require kalimeromk/update-htmldom

## Laravel 5 Setup

1. Add the service provider to `config/app.php`.

```php
'providers' => array(
    ...
	'Htmldom\HtmldomServiceProvider',
    ...
```

2. Add alias to `config/app.php`.

```php
'aliases' => array(	
    ...
	'Htmldom' => 'Htmldom\Htmldom',
    ...
```

## Usage

1. Use following:

```php
$html = new \Htmldom('http://www.example.com');

// Find all images 
foreach($html->find('img') as $element) 
       {echo $element->src . '<br>';}

// Find all links 
foreach($html->find('a') as $element) 
       {echo $element->href . '<br>';}
```

See the detailed documentation http://simplehtmldom.sourceforge.net/manual.htm

s
