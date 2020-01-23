---
title: xor
type: condition
---

<!--
     THIS FILE IS AUTOGENERATED!

     To make changes please edit the contents of:
     lib/condition/xor.go
-->


```yaml
xor: []
```

Returns the logical XOR of its children conditions, meaning it only resolves to
true if _exactly_ one of its children conditions resolves to true.

``` yaml
# True if message contains 'foo' or 'bar', but not both
xor:
  - text:
      operator: contains
      arg: foo
  - text:
      operator: contains
      arg: bar
```

