---
title: Remember about the count limit of CSS selectors in IE
date: "2014-11-15T22:12:03.284Z"
description: ""
---

If you've ever included too many libraries into your CSS build you might have experienced the pure awesomeness of not knowing why your styles disappear in IE 8 and 9 (if you still support the former). Things should be visible in the inspected code and they just aren't there.

The simple reason is the selector count limit. These favorite browsers of ours will only parse the first 4096 selectors and throw the rest out the window.

## Solution

The obvious and straightforward solution is to divide your CSS into smaller chunks. You can either do it by hand or if preprocessors are your thing (and they should be) use a nice piece of plugin magic like [Bless](http://blesscss.com/).

Good luck in your fight. You're not alone!
