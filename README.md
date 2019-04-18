# Hello World - Ruby/Gem
**Ruby Version:**   2.6.1

A simple [hello world gem](https://silverstrange.github.io/2019/04/18/my-first-ruby-gem.html) named 'hola'. Built by following the RubyGem's guide: [Make Your Own Gem](https://guides.rubygems.org/make-your-own-gem/).

To use, add the following to your gem file:

```ruby
gem 'hola', git: 'https://github.com/SilverStrange/hello_world/tree/ruby/gem'
```

To use locally:

```bash
git clone -b ruby/gem --single-branch https://github.com/SilverStrange/hello_world
gem build hola.gemspec
gem install ./hola-0.0.0.gem
irb
```

```ruby
require 'hola'
Hola.hi
```

Expected output:
```
Hello world!
 => nil
```
