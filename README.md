# EBI-Mail-template
E-mail templates and guidance for Mac Mail stationary and Thunderbird message templates

## Mac Mail
Mac Mail uses "[stationary](http://www.instructables.com/id/Easy-Customizing-of-Apple-Mail-Stationary/)".

To make a custom stationary file, download the quick start and you'll need to edit:
- The content
  - File: `template.mailstationery/Contents/Resources/content.html`
  - Note that user-editable areas are wrapped with `<span contenteditable="true" apple-content-name="body"><DIV>`
- Metadata
  - File: `template.mailstationery/Contents/Resources/Description.plist`
  - Update the `Display Name` string
  - Generate a new `Stationery ID` in Terminal by running `uuidgen`
  - Add/remove thumbnail and background files as desired

### Mac Mail stationary FAQs
- Where are system wide templates stored?
  - `/Library/Application Support/Apple/Mail/Stationery/Apple/Contents/Resources/Stationery/Contents/Resources/`
- Where are my templates stored?
  - You shouldn’t need to grab the template directly, but it’s at: `~/Library/Containers/com.apple.mail/Data/Library/Application Support/Mail/Stationery/Apple/Contents/Resources/Custom`
- How do I delete a template?
  - In Mac Mail, open the stationary list and hover over a template, looking for the the "X" to delete



## Compatiblity
| Mail agent     | Recipient client | Pass/fail  |
| ------------- |:-------------:| -----:|
| Mac Mail      | Mac Mail | Pass |
| Mac Mail      | gmail | Pass |
