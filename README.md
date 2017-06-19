[![Build Status](https://travis-ci.org/biztek/hipaa-npi-number-input.svg?branch=master)](https://travis-ci.org/biztek/hipaa-npi-number-input)
[![Sauce Test Status](https://saucelabs.com/buildstatus/biztek)](https://saucelabs.com/u/biztek)
[![Sauce Test Status](https://saucelabs.com/browser-matrix/biztek.svg)](https://saucelabs.com/u/biztek)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/biztek/hipaa-npi-number-input)

_[Demo and API docs](https://biztek.github.io/hipaa-npi-number-input/components/hipaa-npi-number-input)_

# \<hipaa-npi-number-input\>

`<hipaa-npi-number-input>` is a single-line text field to hold valid HIPAA compliant NPI number.

```html
<hipaa-npi-number-input label="Input label"></hipaa-npi-number-input>
```

It includes an optional label,error message,invalid,autovalidate and required attributes.

```html
<hipaa-npi-number-input label="Input label"></hipaa-npi-number-input>
<hipaa-npi-number-input error-message="Invalid input!"></hipaa-npi-number-input>
<hipaa-npi-number-input invalid="boolean value"></hipaa-npi-number-input>
<hipaa-npi-number-input autoValidate="boolean value"></hipaa-npi-number-input>
<hipaa-npi-number-input required="boolean value"></hipaa-npi-number-input>
```
### NPI Numbers Validation

A NPI number (NPI Registration Number) is a number assigned to a health care provider.

A valid NPI number consists of: 9 numbers, & last 1 check digit.

The last Number : NPI numbers can be verified by using the last number, which is known as the Check Digit.

Right Format NPI Number example: 1245319599 .

Wrong Format NPI Number : 1231231231.

### Listening for input changes

By default, it listens for changes on the `bind-value` attribute on its children nodes and perform
tasks such as auto-validating and label styling when the `bind-value` changes.

### Validation

If the `auto-validate` attribute is set, element validates the input whether it is HIPAA compliant NPI number and update
the label styling when the input value changes.

### License

Licensed under [Apache 2.0](LICENSE).
