### rakismet
---
https://github.com/joshfrench/rakismet


```
gem 'rakismet'

```

```ruby
config.rakismet.key = ''
config.rakismet.url = ''

YourApp::Application.config.rakismet.key = ''
YourApp::Application.config.rakismet.url = ''

config.rakismet.proxy_host = ''
config.rakismet.proxy_port = ''

config.rakismet.url = Proc.new {}

class Comment
  include Rakismet::Model
end

class Comment
end

class Comment < ActiveRecord::Base
end

class Trackback
end

config.rakismet.use_middleware = false

config.rakismet.excluded_headers = []

config.rakismet.test = false
config.rakismet.test = true

YourApp::Application.config.rakismet.test = false
YourApp::Application.config.rakismet.test = true

```

```
```

