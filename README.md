# Yatapp

Welcome to Yata integration gem, this gem will allow you to easy get your translations from http://yatapp.com service. 

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'yatapp'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install yatapp

## Usage
Before using Yata integration gem you need to configure it.
We recommend adding the following lines to freshly created initialiser:


```ruby
include Yatapp

Yatapp.configure do |c|
  c.languages         = ['en', 'de'] # add any languages you wish by language code
  c.api_access_token  = ENV['YATA_API_KEY'] # access key to Yata
  c.project           = 'hash-of-your-project' # project you wish to fetch from
end

```


## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release` to create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

1. Fork it ( https://github.com/[my-github-username]/yatapp/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
