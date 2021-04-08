# ProcessDebugPageFields
#### [Processwire](https://processwire.com/) module to debug page fields in a readable manner
---
Adds two new properties to all pages:
- **$page->debugFieldValues** – returns an object with all (sub-)fields, their labels, fieldtypes and values in a readable manner
- **$page->debugFieldTypes** – returns an object with all fieldtypes and their corresponding fields

Both properties are best to be used in combination with debugging tools like [Tracy Debugger](https://processwire.com/modules/tracy-debugger/) or [Ray](https://myray.app/)
