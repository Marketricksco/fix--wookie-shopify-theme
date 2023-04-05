# Wookie Shopify Theme FIX

#### Your store with the Shopify theme Wookie suddenly crash?

Stores with a 2.0.1 or older versions of the template dont load images and components in the storefront.

When you see the DEV TOOLS CONSOLE got two errors:

- Uncaught SyntaxError: Identifier 't' has already been declared
    at theme.js?:1:1
- Uncaught TypeError: $[_0xe319[2]] is not a function vendor.min.js?:19 

(You could see the error in the wookie demo 20 https://wokiee-demos.myshopify.com/?fts=0&preview_theme_id=45876379706)


To fix this issue in your current theme replace the next files called in the include_js.liquid snippet (line 1, line 41):
- theme.js
- vendor.min.js

With recent version of the files (in newer versions of the template)


Or simply replace the include_js.liquid code of this repo for your current include_js.liquid (keep in mind that if you have added custom code it will be overwritten).