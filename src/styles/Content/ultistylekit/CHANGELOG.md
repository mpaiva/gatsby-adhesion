## UltiStyleKit Releases

# 2.1.0

## Major changes

* Add latest revision of button styling from Visual Redesign work
* Add new .form-control sizing classes
* Bump Bootstrap dependency to latest minor release series (3.3.x)
* Allow for custom labels on switch control
* Add new button variant: Circle Buttons
* Changed Default Panel header color to white

## Small revisions and bug fixes

* Avoid double-spacing between label and asterisk on required fields
* Lighten placeholder text in form controls
* Add better browser support to switch control
* Set larger touch-target size on .navbar-toggle
* Added new typography helpers for more flexibility
* Corrected vertical alignment of Brand Image in User Navbar
* Fixed "invisible" text in Warning Labels

# 2.0.0

There have been many changes since v1.0.7 to improve the usability, maintainability, performance, and documentation of the library.

+ Added a **Bower** package.
+ Updated to **Bootstrap 3.2.0**.
+ Reduced CSS selector count by at least 1120.
+ Uses **NodeJS, Bower & Grunt** for portability and ease of installation.
+ Automatically resolves compatible dependencies for Bootstrap & Font-Awesome in NuGet and Bower packages.
+ Added a **ZIP** package.
+ Added a precompiled **ultistylekit.css** which is preconfigured to work in default scenarios for all packages.
+ Developed using best practices defined in [SMACSS](https://smacss.com/) by Jonathan Snook.
+ Tested all packages in actual web projects.

### Breaking Changes from v1.0.7 to v2.0.0

There were several CSS classes that contributed greatly to the size of the CSS being generated. These were removed to improve performance.

```
.error-summary -> .alert.alert-danger
.primary-action -> .btn.btn-primary
.primary-action-lg -> .btn.btn-primary.btn-lg
.secondary-action -> .btn.btn-success
.default-action -> .btn.btn-default

.field -> .form-group
.errors -> .has-error .help-block
form.inline -> .form-inline
form.horizontal -> .form-horizontal
```
