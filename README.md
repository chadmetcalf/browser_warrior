# BrowserWarrior

Are you a warrior to reject your ie 6/7/8 user?

Yes, we should say YES.

**BrowserWarrior** make it super easy.

Make your Ruby on Rails Application rejecting ie6/7/8 with only one line code.

```ruby
# in your Gemfile
gem 'browser_warrior'
```

And then:
```bash
$ bundle
```

Add this code to your `application_controller.rb`:

```ruby
before_action :check_browser_warrior!
```

Then all of ie 6/7/8 user will be rejected to a page that suggests upgrading their browsers.

Upgrading browser screenshot
![screenshot](https://github.com/80percent/browser_warrior/raw/master/img/browser.png)

## More configuration

**QA**: Can I add more unsupported browsers?

Very easy. Execute:

```bash
$ rails g browser_warrior:install
```

It will generate `browser_warrior.rb` in `config/initializers/`.

Edit it.

There is a `browser` object that you can easily custom your requirement.

See more: <https://github.com/fnando/browser#usage>

**QA**: Can I custom the suggested browser page?

Sure. Execute:

```bash
# We are doing more work on it
$ rails g browser_warrior:views
```

It will generate `view` and `css` files for you.
Then edit them.

Easy, is it?

## TODO

* i18n support
* extend support rails 4 or 3.

## Contributing
[windy](https://github.com/windy)

## License
The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
