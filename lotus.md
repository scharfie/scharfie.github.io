# Lotus quick reference/recipes

#### HTML safe string

```ruby
# anywhere
::Lotus::Utils::Escape::SafeString.new(string)

# in a view
_raw string
```
