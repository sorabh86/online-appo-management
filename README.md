# Online Appo Man MCA-mini-project 

A skeleton for creating applications with [CakePHP](https://cakephp.org) 3.5.x.

The framework source code can be found here: [cakephp/cakephp](https://github.com/cakephp/cakephp).

From Xampp Console
### installing
```
php "readfile('https://getcomposer.org/installer');" | php
```
### create new project
```
php composer.phar create-project --prefer-dist cakephp/app myproject
```
### installing using composer.json
```
php composer.phar install
```
### bake table
```
bin\cake bake all <table_name>
```

## HtmlHelper
Folder Template/Layout/default.ctp
```
$this->Html->link(__('Patients'), ['controller'=>'patients', 'action'=>'index']);
```
It will create a link, first argument for text, double underscore function format string, second argument will be an array defined controller and action.

## Element
Folder Template/Element/actions.ctp
```
$this->Element('actions', array('type'=>'Patient','typePlural'=>'Patients'))
```
Here above we include a pre defined template to other views, dynamically providing values.

## Installation
1. Download [Composer](https://getcomposer.org/doc/00-intro.md) or update `composer self-update`.
2. Run `php composer.phar create-project --prefer-dist cakephp/app [app_name]`.

If Composer is installed globally, run

```bash
composer create-project --prefer-dist cakephp/app
```

In case you want to use a custom app dir name (e.g. `/myapp/`):

```bash
composer create-project --prefer-dist cakephp/app myapp
```

You can now either use your machine's webserver to view the default home page, or start
up the built-in webserver with:

```bash
bin/cake server -p 8765
```

Then visit `http://localhost:8765` to see the welcome page.

## Update

Since this skeleton is a starting point for your application and various files
would have been modified as per your needs, there isn't a way to provide
automated upgrades, so you have to do any updates manually.

## Configuration

Read and edit `config/app.php` and setup the `'Datasources'` and any other
configuration relevant for your application.

## Layout

The app skeleton uses a subset of [Foundation](http://foundation.zurb.com/) (v5) CSS
framework by default. You can, however, replace it with any other library or
custom styles.
