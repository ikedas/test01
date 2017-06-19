## Problem Description

In East Asian texts in general, no word separators (spaces) are written explicitly.  So 
```markdown
> 前の**文字列**の後
```
should be rendered as
> 前の**文字列**の後

and this works in practice.

However, if text fragment to be emphasized are ends or starts with punctuation:
```markdown
> 前の**前の「文字列」**の後、前の**「文字列」の後**の後、そのあと。
> 
> 前の**「文字列」**の後。
```
they won't rendered as expected:
> 前の**前の「文字列」**の後、前の**「文字列」**の後、そのあと。
> 
> 前の**「文字列」**の後。

Possible workaround is inserting space before or after punctuations ("␣" means space):
```markdown
> 前の**前の「文字列」**␣の後、前の**␣「文字列」の後**の後、そのあと。
> 
> 前の␣**「文字列」**␣の後。
```
but it will generate ugry text with an extra space before or after punctuations:
> 前の**前の「文字列」** の後、前の **「文字列」の後**の後、そのあと。
> 
> 前の **「文字列」** の後。


