# DetailedSlackNotifier

Welcome to your new gem! In this directory, you'll find the files you need to be able to package up your Ruby library into a gem. Put your Ruby code in the file `lib/detailed_slack_notifier`. To experiment with that code, run `bin/console` for an interactive prompt.

TODO: Delete this and the text above, and describe your gem

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'detailed_slack_notifier'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install detailed_slack_notifier

## Usage

Use it as a [exception_notifier](https://github.com/smartinez87/exception_notification) plugin

```ruby
config.add_notifier :detailed_slack,
  webhook_url: your_slack_webhook
```

```ruby
config.add_notifier :detailed_slack,
  webhook_url: your_slack_webhook,
  username: desired_bot_username,
  channel: desired_destination_channel
```

#### Options

##### webhook_url

*String, required*

The Incoming WebHook URL on slack.

##### channel

*String, optional*

Message will appear in this channel. Defaults to the channel you set as such on slack.

##### username

*String, optional*

Username of the bot. Defaults to the name you set as such on slack

## Development

After checking out the repo, run `bin/setup` to install dependencies. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/coffeebeantech/detailed_slack_notifier. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](http://contributor-covenant.org) code of conduct.


## License

The gem is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
