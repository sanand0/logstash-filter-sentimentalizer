# Logstash Filter Sentimentalizer

This is a plugin for [Logstash](https://github.com/elasticsearch/logstash).

License: Apache 2.0.

## Building

    git clone https://github.com/sanand0/logstash-filter-sentimentalizer.git
    cd logstash-filter-sentimentalizer

    # Change this to your logstash vendor directory path
    export DIR=/usr/share/logstash/vendor

    env GEM_HOME=$DIR/bundle/jruby/1.9 $DIR/jruby/bin/jruby $DIR/bundle/jruby/1.9/gems/bundler-1.9.10/bin/bundle install
    env GEM_HOME=$DIR/bundle/jruby/1.9 $DIR/jruby/bin/jruby $DIR/jruby/bin/gem build logstash-filter-sentimentalizer.gemspec
    sudo /usr/share/logstash/bin/logstash-plugin install logstash-filter-sentimentalizer-0.1.0.gem
