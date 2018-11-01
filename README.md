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

config.rakismet.url = Proc.new { ApplicationController.current_tenant.url }

class Comment
  include Rakismet::Model
end

class Comment
  include Rakismet::Model
  attr_accessor :commenter_name, :commenter_email
  rakismet_attrs :author => :commenter_name, :author_email => :commenter_email
end

class Comment < ActiveRecord::Base
  include Rakismet::Model
  belongs_to :author
  rakismet_attrs :author => proc { author.name },
                 :author_email => proc { author.email }
end

class Trackback
  include Rakismet::Model
  rakismet attrs :comment_type => "trackback"
end

config.rakismet.use_middleware = false

config.rakismet.excluded_headers = ['HTTP_COOKIE', 'HTTP_SENSITIVE']

config.rakismet.test = false
config.rakismet.test = true

YourApp::Application.config.rakismet.test = false
YourApp::Application.config.rakismet.test = true

```

```
```

