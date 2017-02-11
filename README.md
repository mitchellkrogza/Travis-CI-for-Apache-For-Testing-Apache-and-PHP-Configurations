[![Build Status](https://travis-ci.org/mitchellkrogza/Travis-CI-for-Apache-For-Testing-Apache-and-PHP-Configurations.svg?branch=master)](https://travis-ci.org/mitchellkrogza/Travis-CI-for-Apache-For-Testing-Apache-and-PHP-Configurations)
# Template for Travis CI Testing of Apache Configuration Files
## Written by Mitchell Krog - https://github.com/mitchellkrogza

This is a very basic template for getting Travis CI's container based infrastructure to install a stable version of Apache on Ubuntu 14.04 (Trusty) along with PHP 7.0 to test any scenario of apache.conf files and customization scripts you have written. Travis currently only supports Trusty versions of Ubuntu so the PHP 7 packages are pulled in from ppa:ondrej/php

## The purpose of this repository?

Travis CI is a great system for checking and testing your build's Commits, Pull Requests and Merges. Travis runs everything inside a Docker container so it's a fully contained system that you can run build tests on your GIT repository and you can't break anything outside of it.

This repository contains a simple layout for installing Apache and PHP 7.0 into Travis, then loading your config files and running and number of bash commands to test your scripts.

If you pulled all your hair out already trying to get this all to work with Travis CI then you have landed in the right repository. This is a work in progress, rather rough at the edges but it works so far and needs a lot more work done to it still. But I'm sure it will at least guide you in the right direction for testing Apache stuff using Travis CI.

This very basic script tests a curl against a simple file we place into the /var/www directory and then also tests that php is working by running a curl to info.php also placed into the /var/www directory during out Travis build.

If you don't even know what the heck Travis CI is read here - https://travis-ci.org/

### If this helped you why not [buy me a beer](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=BKF9XT6WHATLG):beer: