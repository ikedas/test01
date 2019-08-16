---
redirect_from:
  - ../page.html
---

Page
====
  - tracking => `dsn`&#124;`mdn`&#124;`r`&#124;`w`&#124;`verp`

condition : "!" condition
    &#124; "true" "(" ")"
    &#124; "equal" "(" var "," var ")"
    &#124; "is\_editor" "(" listname "," var ")"
    &#124; "is\_listmaster" "(" var ")"
    &#124; "is\_owner" "(" listname "," var ")"
    &#124; "is\_subscriber" "(" listname "," var ")"
    &#124; "less\_than" "(" var "," var ")"
    &#124; "match" "(" var "," "/" perl\_regexp "/" ")"
    &#124; "newer" "(" date "," date ")"
    &#124; "older" "(" date "," date ")"
    &#124; "search" "(" named\_filter\_file ")"
    &#124; "verify\_netmask" "(" network\_block ")"
    &#124; "CustomCondition::" package\_name "(" var\* ")"
