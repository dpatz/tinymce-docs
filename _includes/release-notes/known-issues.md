
This section describes issues that users of TinyMCE 5.0 may encounter, as well as possible workarounds for these issues.

[Track developer preview issues on GitHub](https://github.com/tinymce/tinymce/labels/5.x)

<!--### Customer reported known and fixed issues

#### TinyMCE 5 kills page responsiveness on Chrome

[Link](https://github.com/tinymce/tinymce/issues/4597)

In TinyMCE Developers Preview version, pages were slow to respond on Chrome. The responsive issue was caused by excessive use of memory when multiple inline editors were used.  This issue was fixed by optimizing the way the inline editor consumes memory.  The inline editor's deactivated state was improved to consume less memory when it was not being used. When the inactive editor becomes active again, its full capabilities are restored.  This optimization resulted in only one active editor consuming memory while the others are in a dormant, ready state.

### Create new UI controls by extending existing ones
[Link](https://github.com/tinymce/tinymce/issues/4588)

Previously, it was possible to create new UI controls by extending existing controls. In the current version of TinyMCE, the UI controls are not exposed in the API directly. Hence, it is not possible to create new UI controls by extending existing controls. This functionality was changed to provide flexible components that did not need to be extended, making it easier to create dialogs that adjust to the active skin. The reduced API surface is also easier to maintain. Based on more customer feedback and use cases, this functionality may be extended to provide more flexibility to create new UI controls.

### UI accessibility issues

#### Insert/Edit image

In TinyMCE Developers Preview version, when the focus was on the source input, the tab did not shift the focus to the source button. This issue was being caused due to the size input lock component not reading dimensions -> width, or dimensions -> height. As a consequence of this issue, image list select box up and down arrow did not change the content. To resolve this issue, the code was restructured to read the the label context. This issue also affected the dialog select component task. This issue has been fixed in the current release of TinyMCE.

#### Context menu component

Previously, when the context menu for a link was opened by pressing the `Shift+F10` keys or right-clicking on the link, pressing `Esc` key closed the context menu. In the current version of TinyMCE, this feature does not work as expected. This issue will be fixed in the future release of TinyMCE.

#### Split button component - num/bullist

Previously, when the focus was on a split button, there were no focus outlines and pressing the `Enter` key created a list item. In the current version of TinyMCE, the split section appears when the `Shift+Enter` keys are pressed without any notifications to the user. The colorpicker and datetime plugins also have the same issue. To fix this issue in the future release of TinyMCE, the operation of opening the menu by pressing the `Shift+Enter` keys will have user notifications.

#### Lists, font color/fore/background, spell checker

In the current version of TinyMCE, There is no way to know if a button is pressed or not. This behavior is expected for the language options when the `Shift+Enter` keys are pressed. This issue will be fixed in the future release of TinyMCE.

#### Spellcheck button

Previously, when the focus was on the spellcheck button, pressing the right arrow key shifted the focus to the next button. In the current version of TinyMCE, this does not work as expected. This issue will be fixed in the future release of TinyMCE.

#### Other UI known issues

The following issues were reported in the current TinyMCE UI:
* In the current version, when English is selected from the language options, there is no tick mark in the UI. This operation is notified through verbal announcement only.
* In the current version, autocorrect does not announce when a word changes.
* In the current version, spelling highlights do not have an attribute `aria-invalid="spelling"` for assistive tools to announce when the cursor has entered a misspelled word.

The above issues will be fixed in the future release of TinyMCE. -->


