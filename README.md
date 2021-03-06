# EolclubScraper

[![Build Status](https://travis-ci.org/PVDTechEvents/eolclub_scraper.png?branch=master)](https://travis-ci.org/PVDTechEvents/eolclub_scraper)

Scrape currently scheduled event from [EOLclub.org](http://eolclub.org/).
Built for automating updates to [PVDTechEvents.com](http://pvdtechevents.com/).

NOTE: Current implementation is extremely fragile, and will very likely break if any changes are made to EOLclub.org's layout.
Use at your own risk.

## Installation

Add this line to your application's Gemfile:

    gem 'eolclub_scraper'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install eolclub_scraper

## Usage

```ruby
require 'eolclub_scraper'
event = EolclubScraper.scheduled_event
event.start_time #=> 2013-12-09 18:00:00 -0500
event.end_time #=> 2013-12-09 23:00:00 -0500
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
