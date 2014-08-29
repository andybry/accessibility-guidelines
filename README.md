# Accessibility Guidelines

This repository is intended to provide guidance in meeting accessibility standards to developers who are implementing 
client side code.

It presents a list of standards that should be met. For each standard, it explains:

1. **What** the standard is.
2. **Why** the standard improves accessibility.
3. How to **Check** that the standard is met.
4. **Examples** of passing and failing code.


## Usage

Any changes to client code should never result in code which causes further breaches of these guidelines.
Any newly implemented code will conform to these guidelines.


## The Guidelines

### 1. W3C standards should be met by HTML and CSS

#### What:

The syntax for HTML and CSS should be correct.


#### Why:

All browsers use the W3C standards to interpret HTML and CSS. Thus, if we want to ensure that a client's browser
is correctly interpreting the code, correct syntax is a minimum requirement. This applies to all the functionality
that we want to deliver, including accessibility.
  
  
#### Check:

For HTML: use the [W3C Validator] to validate any HTML documents that your code will be part of. Documents can be 
checked by external URI, by uploading a file, or by pasting the contents of a file in. There should be no errors, and
as few warnings as possible.


<!-- References -->
[W3C Validator]: http://validator.w3.org/