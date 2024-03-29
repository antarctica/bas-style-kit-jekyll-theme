# BAS Style Kit Jekyll Theme - Change log

All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased][unreleased]

## 0.12.4 - 2023-10-05
### Changed
* Use new versions of css & js etc from the BAS CDN
## 0.12.2 - 2023-08-11
### Added

* Sticky class for sidebar in _layouts/bas-style-kit/bsk--standard-page.html
## 0.12.1 - 2023-08-10
### Fixed

* Syntax error for an offset class in _layouts/bas-style-kit/bsk--standard-page.html

### Added
## 0.12.0 - 2023-07-13

### Added

* Updated to Style Kit 0.7.0-alpha
* Updated to jQuery 3.6.0
* Updated to Jekyll 4.3.2

### Removed

* jQuery 
## 0.11.0 - 2021-03-17

### Added

* Updated to Style Kit 0.6.1
* Updated to jQuery 3.6.0
* Updated to Jekyll 4.2
* Updated Ruby dependencies
* Added optional item type header pattern integration into standard page layout

### Removed

* Synk testing due to incompatibility with modern bundler versions

## 0.10.0 - 2020-06-27

### Added

* Updated to Style Kit 0.6.0-beta
* Updated to JS Cookie 2.2.1
* Updated to jQuery 3.5.1
* Updated to Jekyll 4.1
* Updated Ruby dependencies
* Missing patterns for start and 'sign in' page patterns
* Support for new component patterns (item type header and ORCID iD)

### Changed

* Feedback links changed to open in a new tab
* Updated licence dates
* Updated release procedures

## 0.9.0 - 2019-07-02

### Added

* Updated to Style Kit 0.6.0-alpha

### Fixed

* Updating Gem lock file to fix gem versioning issue
* Correcting use of deprecated `js-libs` in the BAS CDN

### Changed

* Major refactoring and simplification of README and other documentation
* Removing versioning from Docker containers

## 0.8.0 - 2018-11-28

### Added

* Updated dependencies for internal Gem test site
* Updated to Style Kit 0.5.0
* Tracking Gem lock file within project

## 0.7.0 - 2018-11-24

### Added

* 'Problem with this service' (basic) page pattern variant
* 'Problem with this service' (contact) page pattern variant
* 'Problem with this service' (alternative) page pattern variant
* 'Service unavailable' (contact) page pattern variant
* 'Service unavailable' (availability) page pattern variant
* 'Service unavailable' (alternative) page pattern variant
* 'Service unavailable' (partly closed) page pattern variant
* 'Service unavailable' (closed) page pattern variant
* 'Service unavailable' (replaced) page pattern variant
* Updated to Jekyll 3.8.5 to address security vulnerability
* Updated to Style Kit 0.5.0-beta
* Snyk dependency scanning support

### Fixed

* README typo

### Changed

* Improving release procedures

## 0.6.0 - 2018-09-18

### Changed [BREAKING!]

* Icon uses replaced with alternatives or removed where not needed due to the removal of Font Awesome
* Favicon attribute option changed, set `bas_style_kit_jekyll_theme.attributes.head_favicon` to `default` for the Style
  Kit favicon, other values will be ignored and no favicon will be set

### Added

* Updated to Style Kit 0.5.0-alpha
* Implemented Style Kit Favicon
* Implemented 'page not found' pattern and support for design patterns generally
* Implemented 'Service unavailable (basic)' pattern
* Ruby dependencies are now scanned for vulnerabilities using Snyk

### Changed

* Updating order of navigation launcher items
* Improving Dockerfiles
* Improving internal test content

### Fixed

* Corrected link to issue tracker

## 0.5.0 - 2018-07-06

### Fixed

* Ignoring gem lock file to prevent Jekyll runtime errors

### Changed

* Updated to Style Kit 0.4.0
* Changed HR under development phase to dashed line
* Development phase behaviour changed to show experimental phase unless `JEKYLL_ENV` is set to 'production'

## 0.4.0 - 2018-06-14

### Added

* 'is something wrong' and 'back to top' footer includes with optional footer spacer when used with footer content
* Governance statement for use in footers
* Table of Contents (TOC) generic include
* Table of Contents (TOC) Style Kit include
* Page title Style Kit include
* Standard page layout
* Required Jekyll theme directories `_sass` and `assets`
* Legal pages added to gem test site to ensure footer links work as expected

### Changed [BREAKING!]

* Refactored OGL statement as part of the new governance statement footer include, requiring some variable changes
* Upgraded to Style Kit 0.4.0-beta
* Upgraded to Jekyll 3.8.3

### Fixed

* Default URLs to legal policies
* Correcting gem publishing instructions
* Whitespace fixes

### Changed

* Updating order of legal policy links and copyright statement (also changed to 'British Antarctic Survey')
* Updating project copyright from NERC to UKRI

## 0.3.0 - 28/02/2018 - BREAKING!

### Changed [BREAKING!]

* Re-licensing project under the Open Government License
* Upgrading to Jekyll 3.7.2
* Upgrading to Style Kit 0.3.0
* Layouts, includes and data files are now in a `bas-style-kit` namespace
* Generic *blank* and *HTML* layouts and associated includes have been redeveloped
* The Style Kit layout has been split into *base* and *standard* layouts
* Style Kit includes have been redeveloped and renamed
* All data files now use Yaml formatting to support comments

### Removed [BREAKING!]

* *default* layout, switch to either *bsk--base* or *bsk--standard* as needed
* apple touch icons - although these never worked correctly
* 'back to top' and 'is something wrong' links - these will be re-added when supported in the Style Kit
* HTML5 shim and Respond.js as the Style Kit no longer supports IE 10 or below
* All local assets as they are either now part of the Style Kit, or will be re-added when supported in the Style Kit
* Canonical configuration options removed due to removal of canonical HTML meta tag

### Added

* *bsk--base* layout which implements the Style Kit, but in a very generic way
* *bsk--standard* layout which implements the Style Kit with typical elements such as a header and footer
* CSS files are now loaded from a data file, as with JavaScript
* CSS and JavaScript files can and do use Sub-Resource Integrity (SRI) for better security
* Additional CSS and JavaScript files can be added site wide, in addition to specific pages
* Jekyll Menus plugin
* Jekyll Tidy plugin

### Changed

* Upgrading other Gem dependencies to latest versions
* Upgrading application Docker image to use latest BAS Jekyll image
* The *blank* layout is now based on Jekyll's built in *None* layout
* Improving Dockerfile
* Tidying up README
* Tidying up Dockerfile and Docker Compose
* Gemfile lock file is now tracked
* Updated release procedures

## 0.2.3 - 11/04/2017

### Added

* Note in release notes to ensure the Jekyll variable is updated to reflect the changed version

### Fixed

* Error in site-navigation include, where once an item is found to be active, all subsequent items are flagged as well
* Inconsistent indentation in site-navigation include
* Incorrectly displaying active class name instead of screen-reader active element, in drop-down main navigation items

## 0.2.2 - 21/03/2017

### Added

* Jekyll Data plugin as a theme/gem dependency, allows default config options to be set, and the use of theme data files

### Changed

* Including theme config file in Gemspec to allow default config options to be set
* Switching previous config file used for previewing the theme to an internal config file
* Config option documentation is now consistent, and includes whether a default value is set for each option
* Updating theme screen shot

## 0.2.1 - 21/03/2017

### Added

* Test page for loading per-page JavaScript files

### Fixed

* Removing if statement for `body_js_files` front-matter option, which was checking the wrong value and is redundant

### Changed

* Updating release procedures to update theme screen-shot

## 0.2.0 - 20/03/2017

### Added

* Variables data file to provide information about the theme and version of the Style Kit version used for example

### Fixed

* Documenting that the site base URL will be prefixed to navigation item URLs if one is defined

### Changed

* Body JS include now references files from a data file, and allows per-page files to loaded using front-matter
* Updating theme screen shot

## 0.1.2 - 14/03/2017

### Fixed

* Active site navigation item support when using 'pretty' permalinks

## 0.1.1 - Skipped

## 0.1.0 - 12/03/2017

### Added

* Note that the Gem for this project is one minor version ahead of this version due to a technical error
* Initial project - based on BAS Style Kit version 0.1.0, and adapted from the BAS Style Kit documentation Jekyll site