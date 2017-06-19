## Problem Description

In East Asian texts in general, word separators (spaces) never be written explicitly.  So 
```markdown
> 前の**文字列**の後
```
should be rendered as
> 前の**文字列**の後

and in practice this works as expected.

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

## Suggested modification

East Asian punctuations should be treated in the way same as normal East Asian characters (ideographs and so on).

FYI: Most of all of East Asian punctuations are listed here:
* [Requirements for Japanese Text Layout, Appendix A Character Classes](https://www.w3.org/TR/jlreq/#character_classes)
  * Punctuations are categorized in any of A.1 (cl-01) to A.8 (cl-08).
  * Note that ASCII punctuations (e.g. U+0028 parenthesis) listed above must be replaced by their fullwidth counterparts (U+FF08).
  
