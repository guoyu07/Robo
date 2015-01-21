# Composer Tasks

## DumpAutoload


Composer Dump Autoload

``` php
<?php
// simple execution
taskComposerDumpAutoload::_run();

// dump auto loader with custom path
taskComposerDumpAutoload::init('path/to/my/composer.phar')
     ->preferDist()
     ->run();

// optimize autoloader dump with custom path
taskComposerDumpAutoload::init('path/to/my/composer.phar')
     ->optimize()
     ->run();

// optimize autoloader dump with custom path and no dev
taskComposerDumpAutoload::init('path/to/my/composer.phar')
     ->optimize()
     ->noDev()
     ->run();
?>
```










* `optimize()` 


* `preferDist()`  adds `prefer-dist` option to composer
* `preferSource()`  adds `prefer-source` option to composer
* `noDev()`  adds `no-dev` option to composer
* `optimizeAutoloader()`  adds `optimize-autoloader` option to composer



















* `arg($arg)`  Pass argument to executable
* `args($args)`  Pass methods parameters as arguments to executable
* `option($option, $value = null)`  Pass option to executable. Options are prefixed with `--` , value can be provided in second parameter
* `getPrinted()` 
* `dir($dir)`  changes working directory of command
* `printed($arg)`  Should command output be printed




## Install


Composer Install

``` php
<?php
// simple execution
$this->taskComposerInstall()->run();

// prefer dist with custom path
$this->taskComposerInstall('path/to/my/composer.phar')
     ->preferDist()
     ->run();

// optimize autoloader with custom path
$this->taskComposerInstall('path/to/my/composer.phar')
     ->optimizeAutoloader()
     ->run();
?>
```










* `preferDist()`  adds `prefer-dist` option to composer
* `preferSource()`  adds `prefer-source` option to composer
* `noDev()`  adds `no-dev` option to composer
* `optimizeAutoloader()`  adds `optimize-autoloader` option to composer




















* `arg($arg)`  Pass argument to executable
* `args($args)`  Pass methods parameters as arguments to executable
* `option($option, $value = null)`  Pass option to executable. Options are prefixed with `--` , value can be provided in second parameter
* `getPrinted()` 
* `dir($dir)`  changes working directory of command
* `printed($arg)`  Should command output be printed




## Update


Composer Update

``` php
<?php
// simple execution
$this->taskComposerUpdate()->run();

// prefer dist with custom path
$this->taskComposerUpdate('path/to/my/composer.phar')
     ->preferDist()
     ->run();

// optimize autoloader with custom path
$this->taskComposerUpdate('path/to/my/composer.phar')
     ->optimizeAutoloader()
     ->run();
?>
```










* `preferDist()`  adds `prefer-dist` option to composer
* `preferSource()`  adds `prefer-source` option to composer
* `noDev()`  adds `no-dev` option to composer
* `optimizeAutoloader()`  adds `optimize-autoloader` option to composer




















* `arg($arg)`  Pass argument to executable
* `args($args)`  Pass methods parameters as arguments to executable
* `option($option, $value = null)`  Pass option to executable. Options are prefixed with `--` , value can be provided in second parameter
* `getPrinted()` 
* `dir($dir)`  changes working directory of command
* `printed($arg)`  Should command output be printed



