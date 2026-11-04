+++
# Only Works and About are translated, so the en home and taxonomy pages are not rendered
[build]
render = "never"
list = "never"

[[cascade]]
[cascade.build]
render = "never"
list = "never"
[cascade.target]
kind = "{taxonomy,term}"
+++
