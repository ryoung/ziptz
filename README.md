# Ziptz
<!-- [![Version](http://img.shields.io/gem/v/ziptz.svg?style=flat)](https://rubygems.org/gems/ziptz) -->
[![Build Status](http://img.shields.io/travis/infused/ziptz/master.svg?style=flat)](http://travis-ci.org/infused/ziptz)
[![Issues](https://img.shields.io/github/issues/infused/ziptz.svg)](https://github.com/infused/ziptz/issues)
[![Total Downloads](https://img.shields.io/gem/dt/ziptz.svg)](https://rubygems.org/gems/ziptz/)

Get the time zone for any US ZIP code.

<i>ZIP codes are up to date as of <b>June 2015</b>.</i>

## Installation

Add the gem to your Gemfile:

    gem 'ziptz'


## Usage

Get the time zone name for any ZIP code:

    z = Ziptz.new
    z.time_zone_name('97213') #=> "Pacific"

Get the time zone offset for any ZIP code:

    z.time_zone_offset('97213') #=> -8

<i>Please note that offsets do not include daylight savings time.<i>


Get all the zip codes in a time zone:

    z.zips('American Samoa') #=> ["96799", "96941", "96942", "96943", "96944"]


## Supported Time Zones

* "Mountain" GMT -07:00
* "Pacific" GMT -08:00
* "Alaska" GMT -09:00
* "Hawaii-Aleutian Islands" GMT -10:00
* "American Samoa" GMT -11:00
* "Marshall Islands" GMT +12:00
* "Guam" GMT +10:00
* "Palau" GMT +09:00

## License

  Copyright (c) 2015 Keith Morrison <<keithm@infused.org>>

  Permission is hereby granted, free of charge, to any person
  obtaining a copy of this software and associated documentation
  files (the "Software"), to deal in the Software without
  restriction, including without limitation the rights to use,
  copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the
  Software is furnished to do so, subject to the following
  conditions:

  The above copyright notice and this permission notice shall be
  included in all copies or substantial portions of the Software.

  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
  EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
  OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
  NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
  HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
  WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
  FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
  OTHER DEALINGS IN THE SOFTWARE.