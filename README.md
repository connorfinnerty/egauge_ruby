# EgaugeRuby

This gem provides an interface with the Egauge API

## Installation

Add this line to your application's Gemfile:

  `gem 'egauge_ruby', :git => 'git@github.com:Dangeranger/egauge_ruby.git'`

And then execute:

  `$ bundle install`

Or install it yourself as:

```sh
$ git clone
$ gem build egauge_ruby.gemspec
$ gem istall egauge_ruby-version.gem
```

## Usage

Start with a new instance of the Gauge class

  `irb> gauge = Egauge::Gauge.new('http://some_egauge_url.com')`

Call the #current method on the instance of the Gauge class.

  `gauge.current`

  ```ruby
    irb> gauge.current

    >> {
                       "Grid" => -2,
                 "PV Array 1" => 167,
                "PV Array 1+" => 167,
                "PV  Array 2" => 518,
               "PV  Array 2+" => 471,
              "Fans + Halls?" => 44,
            "East front hall" => 28,
            "West front hall" => 1,
                "Recept East" => 0,
                "Recept West" => 0
        }
  ```

## Contributing

1. Fork it ( https://github.com/[my-github-username]/egauge_ruby/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
