EmailComposer
============

email plugin for phonegap(android/ios) .

Installation
------------

### For Cordova 3.0.x:

1. To add this plugin just type: `cordova plugin add https://github.com/MessShawn/emailcomposer.git` or `phonegap local plugin add https://github.com/MessShawn/emailcomposer.git`
2. To remove this plugin type: `cordova plugin remove com.phonegap.plugins.emailcomposer.EmailComposer` or `phonegap local plugin remove com.phonegap.plugins.emailcomposer.EmailComposer`

### NOTE: For older versions of Cordova (You will probably have to use tag 0.2.0)

Usage:
------
Parameters:

callback: never used
subject: a string representing the subject of the email; can be null
body: a string representing the email body (could be HTML code, in this case set isHtml to true); can be null
toRecipients: a js array containing all the email addresses for TO field; can be null/empty
ccRecipients: a js array containing all the email addresses for CC field; can be null/empty
bccRecipients: a js array containing all the email addresses for BCC field; can be null/empty
isHtml: a bool value indicating if the body is HTML or plain text
attachments: a js array containing all full paths to the files you want to attach; can be null/empty
Example

window.plugins.emailComposer.showEmailComposerWithCallback(null,"Look at this photo","Take a look at <b>this<b/>:",["example@email.com", "johndoe@email.org"],[],[],true,["_complete_path/image.jpg", "_other_complete_path/file.zip"]);


