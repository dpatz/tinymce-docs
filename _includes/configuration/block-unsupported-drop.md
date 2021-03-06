## block_unsupported_drop

When the `block_unsupported_drop` option is set to `true`, the editor blocks unsupported images and files from being dropped into the editor. If the `block_unsupported_drop` option is set to `false`, dropping an unsupported file into the editor will cause the browser to navigate away from the page containing the editor.

{{site.requires_5_4v}}

**Type:** `Boolean`

**Default Value:** `true`

**Possible Values:** `true`, `false`

##### Example

```js
tinymce.init({
  selector: 'textarea',  // change this value according to your HTML
  block_unsupported_drop: false
});
```
