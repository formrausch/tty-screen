# TTY::Screen
[![Gem Version](https://badge.fury.io/rb/tty-screen.png)][gem]
[![Build Status](https://secure.travis-ci.org/peter-murach/tty-screen.png?branch=master)][travis]
[![Code Climate](https://codeclimate.com/github/peter-murach/tty-screen.png)][codeclimate]
[![Coverage Status](https://coveralls.io/repos/peter-murach/tty-screen/badge.png)][coverage]

[gem]: http://badge.fury.io/rb/tty-screen
[travis]: http://travis-ci.org/peter-murach/tty-screen
[codeclimate]: https://codeclimate.com/github/peter-murach/tty-screen
[coverage]: https://coveralls.io/r/peter-murach/tty-screen

> Terminal screen size detection which works both on Linux, OS X and Windows/Cygwin platforms and supports MRI, JRuby and Rubinius interpreters.

**TTY::Screen** provides independent screen size detection component for [TTY](https://github.com/peter-murach/tty) toolkit.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'tty-screen'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install tty-screen

## 1. Usage

**TTY::Screen** allows you to detect terminal screen size by calling `size` method which returns [height, width] tuple.

```ruby
screen = TTY::Screen.new

screen.size     # => [51, 280]
screen.width    # => 280
screen.height   # => 51
```

You can also use above methods as class instance methods:

```ruby
TTY::Screen.size  # => [51, 280]
```

## Contributing

1. Fork it ( https://github.com/[my-github-username]/tty-screen/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request

## Copyright

Copyright (c) 2014 Piotr Murach. See LICENSE for further details.
