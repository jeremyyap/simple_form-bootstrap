## master

## 1.4.0

### enhancements
 * Fix JavaScript lints.
 * Tests against newest Rubies.

### bug fixes
 * Fix tests running new RSpec versions.
 * Support Rails 5' attributes API.

## 1.3.0

### enhancements
 * Implement support for token fields. Use the `as: :token` on a Simple Form input field.

### bug fixes
 * Do not change selects to the Bootstrap select class unless they are explicitly select fields. 
   Other types of controls also give select fields -- typeaheads and the like.
 * Fix compatibility layer for Bootstrap selects when the `bootstrap-select-rails` is not installed.

## 1.2.0

### enhancements
  * It allows `submit` buttons to accept blocks. When a block is specified, the submit button will
    use a \<button> tag instead of an \<input> tag. [@lowjoel](https://github.com/lowjoel)

### bug fixes

## 1.1.2

### bug fixes
  * The proper ID for date/time pickers should be generated for non-JavaScript aware browsers first;
    Browsers with JavaScript would reassign the label to the hidden date/time picker. This fixes
    tests written using Capybara, without JavaScript support.
  * Specifying the button size (e.g. `btn-lg`) should still generate the appropriate button class
  (`btn-default` or `btn-primary`). [@lowjoel](https://github.com/lowjoel)

## 1.1.1

Never released.

## 1.1.0

### enhancements
  * There is no longer a need to retain a Simple Form initialiser, as well as a Simple 
  Form-Bootstrap initialiser. Just call `SimpleForm::setup` and the Bootstrap defaults would be 
  automatically applied. [@lowjoel](https://github.com/lowjoel)
  * Started writing specs and running them on Travis!  
