## Sensu-Plugins-skyline

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-skyline.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-skyline)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-skyline.svg)](http://badge.fury.io/rb/sensu-plugins-skyline)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-skyline/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-skyline)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-skyline/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-skyline)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-skyline.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-skyline)

## Functionality

## Files
 * bin/handler-skyline

## Usage
```
{  
  "skyline" : {
     "server" : "skyline.example.com",
     "port" : 2025
  }
}
```
## Installation

Add the public key (if you haven’t already) as a trusted certificate

```
gem cert --add <(curl -Ls https://raw.githubusercontent.com/sensu-plugins/sensu-plugins.github.io/master/certs/sensu-plugins.pem)
gem install sensu-plugins-skyline -P MediumSecurity
```

You can also download the key from /certs/ within each repository.

#### Rubygems

`gem install sensu-plugins-skyline`

#### Bundler

Add *sensu-plugins-disk-checks* to your Gemfile and run `bundle install` or `bundle update`

#### Chef

Using the Sensu **sensu_gem** LWRP
```
sensu_gem 'sensu-plugins-skyline' do
  options('--prerelease')
  version '0.0.1'
end
```

Using the Chef **gem_package** resource
```
gem_package 'sensu-plugins-skyline' do
  options('--prerelease')
  version '0.0.1'
end
```

## Notes
