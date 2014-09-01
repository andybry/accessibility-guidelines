# Accessibility Guidelines

This repository is intended to provide guidance in meeting accessibility standards to developers who are implementing 
client side code.

It presents a list of standards that should be met. For each standard, it explains:

1. **What** the standard is.
2. **Why** the standard improves accessibility.
3. How to **Check** that the standard is met.
4. **Examples** of passing and failing code.
5. **How** to implement.


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

For HTML: use the [W3C HTML Validator] to validate any HTML documents that your code will be part of. Documents can be 
checked by external URI, by uploading a file, or by pasting the contents of a file in. There should be no errors, and
as few warnings as possible.

For CSS: use the [W3C CSS Validator] to validate any CSS files that your code will be part of. Documents can be checked
 by external URI, by uploading a file, or by pasting the contents of a file in. There should be no errors, and as few
 warnings as possible.
 
 
#### Examples: 
 
1. [Failing HTML Validation], the raw HTML is [here][Failing HTML].
1. [Passing HTML Validation], the raw HTML is [here][Passing HTML].
1. [Failing CSS Validation], the raw CSS is [here][Failing CSS].
1. [Passing CSS Validation], the raw CSS is [here][Passing CSS].


#### How:

The HTML and CSS validators both give detailed error messages with explanations of how to fix the problems. Following
this advice should be enough to fix all problems.



### 2. Pages should not contain broken links

#### What:

All links should go to a valid location, including fragment links (URLs ending with a # link).


#### Why: 

Broken links make the site very frustrating to navigate: if you use are using a screen reader then going to a 404 page 
means that you lose your place on the current page. Going back in the browser will often take you back to the 
beginning of the page you came from, at the very least to the last fragment. Broken fragments cause exactly the same
problems because they take you back to the beginning of the page.


#### Check:

Use the [W3C Link Checker]. This will list details about a variety of issues with links on the pages. The two issue
types to avoid are 404 and broken URI fragments. Any 405 codes (method not allowed) need to be checked manually.
 

#### Examples:

1. [Broken Fragment], the raw HTML is [here][Broken Fragment HTML]


<!-- REFERENCES -->
<!-- ======================================================================== -->
<!--                            VALIDATION                                    -->
<!-- ======================================================================== -->
[W3C HTML Validator]: http://validator.w3.org/
[W3C CSS Validator]: http://jigsaw.w3.org/css-validator/
[Failing HTML Validation]: http://validator.w3.org/check?uri=http%3A%2F%2Fandybry.github.io%2Faccessibility-guidelines%2Fexamples%2FW3C%2520standards%2520should%2520be%2520met%2520by%2520HTML%2520and%2520CSS%2Ffailing.html&charset=%28detect+automatically%29&doctype=Inline&group=0
[Failing HTML]: https://raw.githubusercontent.com/andybry/accessibility-guidelines/gh-pages/examples/W3C%20standards%20should%20be%20met%20by%20HTML%20and%20CSS/failing.html
[Passing HTML Validation]: http://validator.w3.org/check?uri=http%3A%2F%2Fandybry.github.io%2Faccessibility-guidelines%2Fexamples%2FW3C%2520standards%2520should%2520be%2520met%2520by%2520HTML%2520and%2520CSS%2Fpassing.html&charset=%28detect+automatically%29&doctype=Inline&group=0
[Passing HTML]: https://raw.githubusercontent.com/andybry/accessibility-guidelines/gh-pages/examples/W3C%20standards%20should%20be%20met%20by%20HTML%20and%20CSS/passing.html
[Failing CSS Validation]: http://jigsaw.w3.org/css-validator/validator?uri=http%3A%2F%2Fandybry.github.io%2Faccessibility-guidelines%2Fexamples%2FW3C%2520standards%2520should%2520be%2520met%2520by%2520HTML%2520and%2520CSS%2Ffailing.css&profile=css3&usermedium=all&warning=1&vextwarning=&lang=en
[Failing CSS]: http://andybry.github.io/accessibility-guidelines/examples/W3C%20standards%20should%20be%20met%20by%20HTML%20and%20CSS/failing.css
[Passing CSS Validation]: http://jigsaw.w3.org/css-validator/validator?uri=http%3A%2F%2Fandybry.github.io%2Faccessibility-guidelines%2Fexamples%2FW3C%2520standards%2520should%2520be%2520met%2520by%2520HTML%2520and%2520CSS%2Fpassing.css&profile=css3&usermedium=all&warning=1&vextwarning=&lang=en
[Passing CSS]: http://andybry.github.io/accessibility-guidelines/examples/W3C%20standards%20should%20be%20met%20by%20HTML%20and%20CSS/passing.css

<!-- ======================================================================== -->
<!--                            BROKEN LINKS                                  -->
<!-- ======================================================================== -->
[W3C Link Checker]: http://validator.w3.org/checklink
