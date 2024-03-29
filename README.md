# Project 3 - Starter Kit - Symfony 4.4.*

# Résumé du projet: #


>Le RHC-CPIAS (Réseau des Hygiénistes du Centre et le Centre d'Appui pour la Prévention des Infections
Associées aux Soins)  souhaite une application web pour faciliter l'inventaire et la diffusion des
BHR. Pour le moment, ce suivi s'effectue à partir d'un fichier national de signalement en ligne
(fichier e-sin) et d'un fichier propre au RHC-CPIAS. Les données sont donc fragmentées, certains
enregistrements n'étant réalisés que dans le fichier national et d'autres uniquement sur le fichier
local, le fichier souche. L'application doit regrouper de ces deux sources en une seule.

>Le RHC-CPIAS est un organisme compétent dans la gestion et le suivi des
bactéries hautement résistantes aux antibiotiques (BHR). Ses missions sont l'appui, la formation et
le conseil aux établissements de santé de la région Centre-Val-de-Loire.

---

![Wild Code School](https://wildcodeschool.fr/wp-content/uploads/2019/01/logo_pink_176x60.png)

It's symfony website-skeleton project with some additional tools to validate code standards.

* GrumPHP, as pre-commit hook, will run 2 tools when `git commit` is run :
  
    * PHP_CodeSniffer to check PSR2 
    * PHPStan will check PHP recommendation
     
  If tests fail, the commit is canceled and a warning message is displayed to developper.

* Travis CI, as Continuous Integration will be run when a branch with active pull request is updated on github. It will run :

    * Tasks to check if vendor, .idea, env.local are not versionned,
    * PHP_CodeSniffer to check PSR2,
    * PHPStan will check PHP recommendation.
    
## Getting Started

### Prerequisites

1. Check composer is installed
2. Check yarn & node are installed

### Install

1. Clone this project
2. Run `composer install`
3. Run `yarn install`

### Working

1. Run `symfony server:start` to launch your local php web server
2. Run `yarn run dev --watch` to launch your local server for assets

### Testing

1. Run `./bin/phpcs` to launch PHP code sniffer
2. Run `./bin/phpstan analyse src --level max` to launch PHPStan
3. Run `./bin/phpmd src text phpmd.xml` to launch PHP Mess Detector
3. Run `./bin/eslint assets/js` to launch ESLint JS linter
3. Run `./bin/sass-lint -c sass-linter.yml` to launch Sass-lint SASS/CSS linter

### Windows Users

If you develop on Windows, you should edit you git configuration to change your end of line rules with this command :

`git config --global core.autocrlf true`

## Deployment

Add additional notes about how to deploy this on a live system


## Built With

* [Symfony](https://github.com/symfony/symfony)
* [GrumPHP](https://github.com/phpro/grumphp)
* [PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer)
* [PHPStan](https://github.com/phpstan/phpstan)
* [PHPMD](http://phpmd.org)
* [ESLint](https://eslint.org/)
* [Sass-Lint](https://github.com/sasstools/sass-lint)
* [Travis CI](https://github.com/marketplace/travis-ci)

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning


## Authors

Wild Code School trainers team

## License

MIT License

Copyright (c) 2019 aurelien@wildcodeschool.fr

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Acknowledgments




