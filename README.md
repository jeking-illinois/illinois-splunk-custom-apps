# uofi_urb_template_APP
Template to create new apps for Splunk Cloud.

Download this folder and add it to a locally running Splunk instance, %SPLUNK_HOME%\etc\apps\uofi_urb_template_APP 
First make a copy of the folder & all its contents to %SPLUNK_HOME%\etc\apps\<APP NAME>_APP
Make any and all changes necessary to %SPLUNK_HOME%\etc\apps\<APP NAME>_APP\default\app.conf, change the icons or logos in %SPLUNK_HOME%\etc\apps\<APP NAME>_APP\static\, and add any additional scripts or KOs to %SPLUNK_HOME%\etc\apps\<APP NAME>_APP\bin\ or %SPLUNK_HOME%\etc\apps\<APP NAME>_APP\default\
Back in %SPLUNK_HOME%\ run the following at the CLI

> splunk package app <APP NAME>_APP

The file will be saved to %SPLUNK_HOME%\etc\system\static\app-packages\<APP NAME>_APP.spl and will automatically have all the proper permissions assigned to all the package so it can be uploaded to Splunk Cloud without issue.
