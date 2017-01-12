# Sugar Labs Contact Preference

Sugar Labs Contact Preference provides a new data type that helps users know how a contact prefers to be contacted, and if they are available to be contacted. An icon is show representing the desired contact preference type. Based on a Do Not Call/Contact flag teh icon can also show a red/green coloring. Red for do not call, green for ok to call. A text area is included to record notes for a do not call reason. If maintained and the contact is marked as Do Not Call, the reason will be shown upon mouse-over of the contact preference icon.

## Installation & Use
* Download the latest .tgz package here: https://github.com/sugarcrmlabs/ContactPreference/releases/latest
* Load the package in your target instance using Module Loader
* Log in as an admin user
* Go to Studio and view the Fields for the Contacts module
* You will see two new custom fields that have been added automatically. 'Contact Status' and 'Contact Preference'. 'Contact Status' is a field of type 'do_not_call_image' that shows an icon representing what is selected in the field 'Contact Preference'. 'Contact Preference' is a DDLB (drop down list box) field, utilizing a new list definition 'contact_methods_list', representing possible contact options. For example, methods like Mobile, Office, Fax, Skype, etc.
* To use these fields you will have to add them to the desired layouts.
* The Red/Green coloring for Do Not Contact status utilizes the OOTB field do_not_call

## Adding to modules other than Contacts
* Go to Studio and view the Fields for the desired module
* Add a field of data type 'Do Not Call Image'
* Add a second field of type DDLB, using the list type 'contact_methods_list'
* If you want to use the Red/Green coloring for Do Not Contact status, you will need to add a field of type checkbox and name it do_not_call (Sugar will automatically add a '_c '. This is ok.)
* Then add fields to the needed layouts
```

## Contributing
Everyone is welcome to contribute to this project! If you make a contribution, then the [Contributor Terms](CONTRIBUTOR_TERMS.pdf) apply to your submission.

Please check out our [Contribution Guidelines](CONTRIBUTING.md) for helpful hints and tips that will make it easier for us to accept your pull requests.

-----
Copyright (c) 2016 SugarCRM Inc. Licensed by SugarCRM under the Apache 2.0 license.
