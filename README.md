# Debug Page Fields
#### [Processwire](https://processwire.com/) module to debug page fields in a readable manner
---
Adds two new properties to all pages:
- **$page->debugFieldValues** – returns an object with all (sub-)fields, their labels, fieldtypes and values in a readable manner
- **$page->debugFieldTypes** – returns an object with all fieldtypes and their corresponding fields

Both properties are best to be used in combination with debugging tools like [Tracy Debugger](https://processwire.com/modules/tracy-debugger/) or [Ray](https://myray.app/)

## Supported fieldtypes
- Button
- Checkbox
- Color
- Combo
- Datetime
- Email
- FieldsetPage *
- File
- FontIconPicker
- Functional
- Image
- ImageReference
- MapMarker
- Multiplier
- Mystique
- Options
- Page
- PageIDs
- PageTitle
- Radio
- Repeater *
- RepeaterMatrix *
- RockAwesome
- SeoMaestro
- Table
- Text
- Textarea
- Textareas
- Toggle
- URL

\* The fields with complete subfield-support also list their corresponding subfields.
