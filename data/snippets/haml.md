```
$echo "%div{:style => "color:red"} hello world" >> test.haml
$coala --files test.haml --bears HAMLLintBear --save
Executing section cli...

test.haml
[   1] %div{:style·=>·"color:red"}·hello·world
**** HAMLLintBear [Section: cli | Severity: NORMAL] ****
!    ! InlineStyles: Do not use inline style attributes
[    ] *0. Do (N)othing
[    ]  1. (O)pen file
[    ]  2. Add (I)gnore comment
[    ] Enter number (Ctrl-D to exit): Found EOF. Exiting gracefully.
$
```
