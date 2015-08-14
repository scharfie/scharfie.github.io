# Lotus quick reference/recipes

#### HTML safe string

```ruby
# anywhere
::Lotus::Utils::Escape::SafeString.new(string)

# in a view
_raw string
```

#### Render a specific view

```ruby
# in this case we are rendering a custom 'shared/error' view,
# in html format, and exposing a variable named 'foo' with value 'bar'
html = Web::Views::Shared::Error.render(:format => :html, :foo => :bar)

# and in a controller, you can make it the response
# (setting `body` will prevent default rendering)
self.body = html
```
