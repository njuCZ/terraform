---
layout: "language"
page_title: "include - Functions - Configuration Language"
sidebar_current: "docs-funcs-string-include"
description: |-
  The include function determines whether a given string may be found within another string.
---

# `include` Function

-> **Note:** This page is about Terraform 0.12 and later. For Terraform 0.11 and
earlier, see
[0.11 Configuration Language: Interpolation Syntax](../../configuration-0-11/interpolation.html).

`include` returns whether a substring is within another string.

```hcl
include(string, substr)
```

## Examples

```
> include("hello world", "wor")
true
```

```
> include("hello world", "wod")
false
```
