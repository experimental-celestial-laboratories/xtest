# xtest: The XNL testing API

Xtest was created to allow in-order testing of Lua scripts with a simple API. It contains assertions for rougly everything that could need to be tested: types, values, function results, errors, Etc.

## Getting Started

Create a test file and require `xtest`.

The tests are ran by the `xtest.run` function, which takes a table of names followed by functions. These will be your test cases.

example:
```lua
local success, result = xtest.run({
  "Assert true succeeds",
  function()
    x.assert(true, "Always succeeds")
  end
})
```
