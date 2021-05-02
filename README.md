# Postgresql migration PHP

> This repo is an example of preparation of a bundle consisting of Composer — PHP packet manager and Swiftmailer app, which your team can use later ensuring software similarity.   

## Usage 
### Check Composer version
```bash
composer
```
### Install some version of Swiftmailer
```bash
composer require swiftmailer/swiftmailer:6.2.0
```
### Update Swiftmailer to the latest version
```bash
composer update swiftmailer/swiftmailer:6.2.7
```
> Add Vendor folder to .gitignore file before committing to remote.   
> Push to remote. 
###  What does your team mate do?
They install php, clone your repo built on the basis of this example repo and install all the software listed in composer.json and dependencies listed in composer.lock.
```bash
composer install
```

## Installation
### PHP on MacOS
Install PHP first!
```bash
brew install php
```
### Composer (locally) (Linux or MacOS)
```bash
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
php -r "if (hash_file('sha384', 'composer-setup.php') === '756890a4488ce9024fc62c56153228907f1545c228516cbf63f885e036d37e9a59d27d63f46af1d4d07ee0f76181c7d3') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
php composer-setup.php
php -r "unlink('composer-setup.php');"
```

## Acknowledgments

This repo was inspired by [skillfactory.ru](https://skillfactory.ru/devops#syllabus) team

## See Also
- [PHP](https://www.php.net/)
- [Composer](https://getcomposer.org)
- [Packagist — package list](https://packagist.org)
- [Composer cheat sheet in Russian](https://phpprofi.ru/blogs/post/52)

## License
Follow all involved parties licenses terms and conditions.