# Practising the `nvim-surround` Plugin

Detailed information on how to use this plugin can be found in `:h nvim-surround.usage`


## Basics

Wrap the following text to match the below text:

```python
string = Hello
require"nvim_surround"
c = x;
int a[] = 32;
```

```python
string = "Hello"
require("nvim-surround")
c = 'x';
int a[] = {32};
```

Hint: `ys{motion}{character}`
ys stands for "you surround"


Delete the following delimiters to match the below text:

```python
local x = ({ 32 })
See `:h help`
local str = [[Hello]]
```

```text
local x = { 32 }
See :h help
local str = [Hello]
```

Hint: `ds{char}`
ds stands for delete surrounding

Change the following delimiters to match the below text:

```text
'some string'
use<"hello">
`some text`
```

```text
"some string"
use("hello")
{some text}
```

Hint: `cs{target}{replacement}`
cs stands for change surrounding {target} into {replacement}
