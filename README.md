# Packer Rails 2.3

> A legacy base box for usage with ruby 1.8 and Rails 2.3

## Installation

The built box is hosted on [Atlas](https://atlas.hashicorp.com/franklinkim/boxes/rails-2.3)

```
$ vagrant box add franklinkim/rails-2.3
```

## Usage

Use it with your `Vagrantfile`:

```
# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  # Every Vagrant virtual environment requires a box to build off of.
  config.vm.box = 'franklinkim/rails-2.3'
end
```

## Building

```
$ git clone https://github.com/franklinkim/packer-rails-2.3.git
$ cd packer-rails-2.3
$ rake build
```

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests and examples for any new or changed functionality.

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## License
Copyright (c) franklin under the MIT license.
