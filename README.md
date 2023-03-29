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
- Decimal
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

If Ray is found in the project (aka the class Spatie\Ray\Ray is loaded), three additional methods will be added to the ray() function:
1. ray()->page($optionalParameter): the Parameter variable can be used as following:
   - None: get infos of the current page 
   - Page ID: get page infos via the page ID
   - Page object: get page infos via a $page variable
   - Field name: get debug infos of a specific field from the current page by providing its name
2. ray()->pages($mandatoryParameter): the Parameter variable can be used as following:
   - Selector: Provide a selector string to find the corresponding pages
   - Pages Object
3. ray()->config($optionalParameter): the Parameter variable can be used as following:
   - None: get all config properties 
   - Property name: get only the value of the provided property
