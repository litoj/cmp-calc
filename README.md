# cmp-calc

nvim-cmp source for math calculation.

# Setup

1. Add the plugin to `nvim-cmp` dependency list.
2. Add it as a source:

```lua
require'cmp'.setup {
  sources = {
    { name = 'calc' }
  }
}
```

3. Type a math expression anywhere or use a method as defined in lua `math` table.

```lua
-- compute and replace ('|' means the cursor position)
your(code, 2.5*log10(100)|) -> your(code, 5|)
-- or append just the result
sqrt(2)^2| -> sqrt(2)^2 = 2|
```
