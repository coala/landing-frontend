```
$ echo "if true
    print('Hello World')
end
" > hello.lua
$ coala --files hello.lua --bears LuaLintBear
Executing section cli...

hello.lua
|   2| ····print('Hello·World')
|    | [MAJOR] LuaLintBear (011):
|    | expected 'then' near 'print'
|    | *0: Do nothing
|    |  1: Open file(s)
|    |  2: Add ignore comment
|    | Enter number (Ctrl-D to exit): <ENTER>
1 $
```
