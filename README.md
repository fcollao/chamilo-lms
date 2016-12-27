# Chamilo 2.x

[![Build Status](https://travis-ci.org/chamilo/chamilo-lms.svg?branch=1.11.x)](https://travis-ci.org/chamilo/chamilo-lms)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/chamilo/chamilo-lms/badges/quality-score.png?b=1.11.x)](https://scrutinizer-ci.com/g/chamilo/chamilo-lms/?branch=1.11.x)
[![Code Coverage](https://scrutinizer-ci.com/g/chamilo/chamilo-lms/badges/coverage.png?b=1.11.x)](https://scrutinizer-ci.com/g/chamilo/chamilo-lms/?branch=1.11.x)
[![Bountysource](https://www.bountysource.com/badge/team?team_id=12439&style=raised)](https://www.bountysource.com/teams/chamilo?utm_source=chamilo&utm_medium=shield&utm_campaign=raised)
[![Code Consistency](https://squizlabs.github.io/PHP_CodeSniffer/analysis/chamilo/chamilo-lms/grade.svg)](http://squizlabs.github.io/PHP_CodeSniffer/analysis/chamilo/chamilo-lms/)
[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/166/badge)](https://bestpractices.coreinfrastructure.org/projects/166)

## Installation

The installation instructions are located in the documentation here: 
[Installation](app/Resources/installation.md)

## Upgrade
The upgrade instructions are located in the documentation here: 
 [Upgrade](https://github.com/chamilo/chamilo-lms/blob/master/app/Resources/upgrade.md)

## Changes from 1.x 

* app/Resources/public/assets moved to web/assets
* main/inc/lib/javascript moved to web/js
* main/img/ moved to web/img
* Installation url changed from main/install/index.php to web/install.php
* main/template/default moved to src/Chamilo/CoreBundle/Resources/views
* Template twig file names are changed from *.tpl to *.html.twig to follow Symfony2 format
* bin/doctrine.php changed to app/console
* php files are now loaded using the web/app_dev.php file
 * In 1.x:
      main/admin/user_list.php
 * In 2.x (dev mode)
      web/app_dev.php/main/admin/user_list.php
 * In 2.x: (prod mode)
      web/main/admin/user_list.php
* Language list is now loaded using the iso code not the english name.
  Example: "es" instead of "spanish" 
* PHPMailer replaced with Swift Mailer
 
  
## Todo
* Template system to work with current Symfony2 structure
* Auth (CAS, Shibboleth, Oath2) 
* URL course changes "cidReq" to "c", "session_id" to "s"
* Fix plugins that use api_get_setting directly in the code


## Contributing

If you want to submit new features or patches to Chamilo, please follow the
Github contribution guide https://guides.github.com/activities/contributing-to-open-source/
and our CONTRIBUTING.md file.
In short, we ask you to send us Pull Requests based on a branch that you create
with this purpose into your repository forked from the original Chamilo repository.

## Documentation
For more information on Chamilo, visit https://1.11.chamilo.org/documentation/index.html
