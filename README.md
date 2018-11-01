### rakismet
---
https://github.com/joshfrench/rakismet


```
gem 'rakismet'

```

```ruby
config.rakismet.key = 'your wordpress key'
config.rakismet.url = 'http://yourdomain.com/'

YourApp::Application.config.rakismet.key = 'your wordpress key'
YourApp::Application.config.rakismet.url = 'http://yourdoamin.com/'

config.rakismet.proxy_host = 'http://yourdomain.com/'
config.rakismet.proxy_port = '8080'

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

