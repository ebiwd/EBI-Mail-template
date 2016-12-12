# EBI-Mail-template
E-mail templates and guidance for Mac Mail stationary and Thunderbird message templates

## Tips
- Analytics: 
  - If you're using Google Analytics, tt's a good idea to track links with the custom URL builder: https://support.google.com/analytics/answer/1033867?hl=en
  - To track e-mail opens, use images with specific files names (a la: `2016-winter-campaign.gif`) and use server-side tracking.

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
  
### Installing a template
Just double click the `filename.mailstationery` file and Mac Mail will prompt you to install. Or if the template is already installed, it will just make a new draft message.

### Mac Mail stationary FAQs
- Where are system wide templates stored?
  - `/Library/Application Support/Apple/Mail/Stationery/Apple/Contents/Resources/Stationery/Contents/Resources/`
- Where are my templates stored?
  - You shouldn’t need to grab the template directly, but it’s at: `~/Library/Containers/com.apple.mail/Data/Library/Application Support/Mail/Stationery/Apple/Contents/Resources/Custom`
- How do I delete a template?
  - In Mac Mail, open the stationary list and hover over a template, looking for the the "X" to delete

## Thunderbird
Thunderbid uses "[Message templates](http://kb.mozillazine.org/Message_templates)" and it is a much simpler afair, consisting of one HTML-like .eml file.

Just download the sample template and edit as you like.

### Installing a template
Save the `template.eml` file and drag it to the desired mailbox's "Templates" folder.

### Thunderbird template FAQs
- Where are system wide templates stored?
  - In the associate mailbox's "Templates" folder
- How do I delete a template?
  - Just delete the "message" from the "Templates" folder

## Outlook
To come, but here's basic guidance on making templates in Outlook: https://support.office.com/en-us/article/Create-an-email-message-template-43EC7142-4DD0-4351-8727-BD0977B6B2D1

Note Outlook on Mac [does not support e-mail templates](https://support.office.com/en-gb/article/Can-I-create-email-templates-in-Outlook-2016-for-Mac-6339b60e-2e5a-4aed-a9e6-2e7b5d7eb5a0).





## Compatiblity
| Mail agent     | Recipient client | Pass/fail  |
| ------------- |:-------------:| -----:|
| Mac Mail      | Mac Mail | Pass |
| Mac Mail      | gmail | Pass |
