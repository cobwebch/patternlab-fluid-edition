Pattern Lab Fluid Edition for Cobweb
====================================

**This package is a fork of NameLessCoder Patternlab Fluid Edition!**

[Check here for current version](https://github.com/NamelessCoder/patternlab-fluid-edition)
 

# Installing

IF some questions are asked during update process, choose "yes" everytime
## Short story

    cd install/location/
    git clone https://github.com/cobwebch/patternlab-fluid-edition.git your-project-name && cd $_
    composer update
    composer generate
    composer server

*When installing, tap "ENTER" each time composer asks you something

Then open [http://localhost:8080](http://localhost:8080) in your browser

## Long story

### Use Composer to create a project

Pattern Lab uses [Composer](https://getcomposer.org/) to manage project dependencies.

#### 1. Install Composer

Please follow the directions for [installing Composer](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx) on the Composer website.

#### 2. Install the Pattern Lab Fluid Edition

Use Composer's [`create-project` command](https://getcomposer.org/doc/03-cli.md#create-project) to install the edition as base for new projects:

    cd install/location/
    composer create-project cobwebch/patternlab-fluid-edition your-project-name && cd $_

This will create a folder named `your-project-name`, install the Fluid edition to that folder and walk you through the install process.

You will be asked to choose a starter kit - at the current time only one such starter kit is available. Select and install it to complete the installation process. 

# Updating Pattern Lab

Updating the Fluid edition of Pattern Lab can be done with `composer update`.


# Helpful Commands

These are some helpful commands you can use on the command line for working with Pattern Lab.

## List all of the available commands

To list all available commands type:

    php core/console --help

To list the options for a particular command type:

    php core/console --help --[command]

## Generate Pattern Lab

To generate the front-end for Pattern Lab type:

    php core/console --generate

## Watch for changes and re-generate Pattern Lab

To watch for changes and re-generate the front-end for Pattern Lab type:

    php core/console --watch

## Start a server to view Pattern Lab

You can use PHP's built-in web server to review your Pattern Lab project in a browser. In a seperate window type:

    php core/console --server

Then open [http://localhost:8080](http://localhost:8080) in your browser.

## Install a StarterKit

To install a near-empty StarterKit as a starting point for your project type:

    php core/console --starterkit --init

To install a specific StarterKit from GitHub type:

    php core/console --starterkit --install <starterkit-vendor/starterkit-name>

