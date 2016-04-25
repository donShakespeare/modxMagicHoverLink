# modxMagicHoverLink.js
An ingenious way to use TinyMCE to do the infamous thing called, internal linking.
A replacement to the TinyMCE `link` plugin, backend only.
While using pdoTools to populate *link_list* is great for backend/frontend, some users asked for a little backend magic that harnesses the existing power of MODX; then modxMagicHoverLink was born.

Hover over Resources in Resource Tree, MODX Manager search result, Link List (backend/frontend)

Full Markdown support for inserting links and images from file browser

Insert MODX internal links with scheme (abs, relative, http, https)

#Usage
```html
  tinymce.init({
    external_plugins: {
      modxMagicHoverLink: "[[++assets_url]]components/tinymcewrapper/tinymceplugins/modxMagicHoverLink.js"
    },
    toolbar: "link unlink",
    //hoverStripMODXurl:false, //default is true
    //hoverAddCLASStoTree:false //default is true
  });
  ```
  In `TinymceWrapper`, to affect all editors at once, call `external_plugins: {...` in your `TinymceWrapperCommonCode` chunk.<br> Or else, make the call in your individual init chunks.

