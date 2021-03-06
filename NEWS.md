# CHANGES IN pagedown VERSION 0.3

## MAJOR CHANGES

- Paged.js is upgraded from version 0.1.28 to 0.1.32: Paged.js CSS variables are now prefixed with `pagedjs-`. For instance, `--width` is replaced by `--pagedjs-width`. Users' stylesheets that use Paged.js CSS variables need to be updated. Bleeds and crop marks are now supported. Several bugs are fixed.

## BUG FIXES

- browser is forced to redraw the document after Paged.js finished. This will fix wrong page references observed with Chrome and RStudio 1.2.xxxx (#35 and #46, thanks, @petermeissner).  

- `jsonlite::toJSON()` is now used in `chrome_print()` for building all the JSON messages sent to headless Chromium/Chrome: this guarantees that the JSON strings are valid (thanks, @ColinFay, #85 and @cderv, #88).


# CHANGES IN pagedown VERSION 0.2

## MAJOR CHANGES

- The function `chrome_print()` has been significantly enhanced. Now it prints web pages and R Markdown documents to PDF through the Chrome DevTools Protocol instead of the simple command-line call (like in v0.1). It also supports capturing screenshots.


# CHANGES IN pagedown VERSION 0.1

## NEW FEATURES

- The first CRAN release. See more information about this package at: https://github.com/rstudio/pagedown.
