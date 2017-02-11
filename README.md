# Template for Travis CI Testing of Apache Configuration Files
## Written by Mitchell Krog - https://github.com/mitchellkrogza

This is a very basic template for getting Travis CI's container based infrastructure to install a stable version of Apache on Ubuntu 16.04 (Xenial) along with PHP and MYSQL to test any scenario of apache.conf files and customization scripts you have written.

## The purpose of this repository?

Travis CI is a great system for checking and testing your build's Commits, Pull Requests and Merges. Travis runs everything inside a Docker container so it's a fully contained system that you can run build tests on your GIT repository and you can't break anything outside of it.

This repository contains a simple layout for installing Apache, PHP and MYSQL into Travis, then loading your config files and running and number of bash commands to test your scripts.

If you pulled all your hair out already trying to get this all to work with Travis CI then you have landed in the right repository.

If you don't even know what the heck Travis CI is read here - https://travis-ci.org/
