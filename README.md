# Software distribution via Composer files

> This repo is a couple of files installing Swiftmailer app by means of Composer — PHP packet manager for ensuring software similarity among php team members.   

## Usage 
### Check Composer version
```bash
composer
```
### Install some version of Swiftmailer
```bash
composer require swiftmailer/swiftmailer:6.2.0
```
### Update Swiftmailer to the latest version if you need
It should go smoothly with
```bash
composer update
```
but for some reason beyond my understanding `composer update` command didn't work for me.  
I edited `composer.json` file by changing `6.2.0` version to `6.2.7` version, save this file, and run a command:
```bash
composer update --with-all-dependencies
```
> Add `Vendor` folder and `composer.phar` file to `.gitignore` before committing and pushing to remote.   

###  What does your team mate do?
1. Install PHP.
2. Create a dir for a project.
3. Install Composer locally to that dir.
4. Clone your repo built on the basis of this example repo in their dir. 
> Don't miss the dot at the end of the command !
```bash
git clone https://github.com/<whatever>.git .
```
 5. Install all the software listed in `composer.json` and dependencies listed in `composer.lock` file.
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
cd /your_project
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