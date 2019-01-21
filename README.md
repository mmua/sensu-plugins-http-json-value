## Sensu-Plugins-http

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-http.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-http)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-http.svg)](http://badge.fury.io/rb/sensu-plugins-http)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-http/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-http)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-http/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-http)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-http.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-http)

## Functionality

## Files
 * bin/check-http-json-value.rb

## Usage

 Can be used to test json values

## Installation

[Installation and Setup](http://sensu-plugins.io/docs/installation_instructions.html)

## Notes

### check-http.rb and check-https-cert.rb
This check is not really geared to check all of the complexities of ssl which is why there is a separate repo and set of checks for that: https://github.com/sensu-plugins/sensu-plugins-ssl. If you are trying to verify cert expiration you will notice that in some cases it does not do what you always expect it to do. For example it might appear that when using using `-k` option you see different expiration times. This is due to the fact that when using `-k` it does not check expiration of all of the certs in the chain. Rather than duplicate this behavior in this check use the other repo where we handle those more complicated ssl checks better. For more information see: https://github.com/sensu-plugins/sensu-plugins-http/issues/67
