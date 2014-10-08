# Ukigumo2

Ukigumo2 is a super lightweight CI server

<img src="https://raw.githubusercontent.com/ukigumo/ukigumo2/master/docs/screenshot.png">

## How do I use this?

Run the ukigumo2 server.

    $ UKIGUMO_SECRET=s3c4et RACK_ENV=production PORT=20080 bundle exec bin/ukigumo2

You can register job by HTTP API.

    $ curl http://localhost:4567/api/enqueue\?repository=https://github.com/miyagawa/Acme-YakiniQ.git

Worker thread executes your application... You can look the execution result on the web.

## Installation

    $ git clone https://github.com/ukigumo/ukigumo2.git
    $ cd ukigumo2
    $ gem install bundler
    $ bundle install
    $ bundle exec ./bin/ukigumo2

## Contributing

1. Fork it ( https://github.com/tokuhirom/ukigumo2/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
