---
layout: default
title: Word Count plugin
title_nav: Word Count
description: Show a word count in the TinyMCE status bar.
keywords: wordcount
---

The Word Count plugin adds the functionality for counting words to the {{site.productname}} editor by placing a counter on the right edge of the status bar. Clicking **Word Count** in the status bar switches between counting words and characters. A dialog box with both word and character counts can be opened using the menu item situated in the **Tools** drop-down, or the toolbar button.

**Type:** `String`

##### Example

```js
tinymce.init({
  selector: "textarea",  // change this value according to your HTML
  plugins: "wordcount",
  toolbar: "wordcount"
});
```

## API

The Word Count plugin exposes an API for retrieving the word and character count of either the whole document or the current editor selection. Following is an example of how to retrieve each property.

##### Example

```js
var wordcount = tinymce.activeEditor.plugins.wordcount;

console.log(wordcount.body.getWordCount());
console.log(wordcount.body.getCharacterCount());
console.log(wordcount.body.getCharacterCountWithoutSpaces());

console.log(wordcount.selection.getWordCount());
console.log(wordcount.selection.getCharacterCount());
console.log(wordcount.selection.getCharacterCountWithoutSpaces());
```
