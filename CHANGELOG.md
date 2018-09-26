# Changelog

## 2.1.0

This release adds major changes to how CSS resets, typography, spacing, and components work in Pine. It is inspired by the approach in our [Acorn framework](https://github.com/ThemeMountain/acorn).

### Highlights

* Smarter CSS resets => less inlined styles when your ESP does automatic inlining
* Better button visuals for Outlook: using `mso-padding-alt` to keep the looks consistent with more modern email clients
* More flexible mobile spacing utilities
    * Spacers and Dividers also allow for more control on mobile
* New breakpoint for landscape phones
* Better image resets

#### Added

* New breakpoint (`max-width: 730px`), for landscape phones. Column widths stay the same as for desktop, but container is forced to 100% width

#### Updated

* All examples and components, to use the new CSS
* Outlook VML backgrounds - not using `<v:fill>` anymore (not needed for them to work)
* Spacers now use `&zwnj;` instead of `&nbsp;`
* Spacers on mobile are reset to zero-height. Use the new mobile spacing utilities to define how high a spacer should be on mobile (up to 60px)
* Renamed `body-bkg-image.html` example to `vml-body-bkg-image.html`

#### Removed

* Double `<head>` hack for Yahoo! on mobile

## 2.0.0

Pine has been re-written (almost) from scratch, to make it more user friendly and flexible.

## 1.0.1

#### Added

* This changelog
* `cellspacing="0"` on all tables
* Meta tag to prevent iOS 11 Mail message reformatting (zoomed-out layout)

#### Updated

* [Documentation](https://thememountain.github.io/pine/)
* Typography reset
* Responsive image CSS
* Nested row tables width reset
* Renamed the 'Standard' grid to 'Boxed'
* Moved inline min-width wrapper table style to embedded CSS
* Moved inline `position` style for hamburger menus to embedded CSS
* Simplified spacers and dividers: removed inline `font-size` and `mso-line-height-rule` styles (the latter has been moved to embedded CSS)

#### Removed

* Outlook.com hamburger menu icon hack

## 1.0.0

🌲 Initial release.
