# modxMagicHoverLink.js
An ingenious way to use TinyMCE to do the infamous thing called, internal linking.
A replacement to the TinyMCE `link` plugin

#Usage
```html
  tinymce.init({
    external_plugins: {
      modxMagicHoverLink: "[[++assets_url]]components/tinymcewrapper/tinymceplugins/modxMagicHoverLink.js"
    }
  });
  ```
  In `TinymceWrapper`, to affect all editors at once, call `external_plugins: {...` in your `TinymceWrapperCommonCode` chunk.<br> Or else, make the call in your individual init chunks.

