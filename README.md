# You've Got Leads Webform
You've Got Leads Contact Save RESTful API integration with Drupal 7 Webforms.

Version 7.x-0.3-dev

## About
Integrates You've Got Leads CRM /leads RESTful endpoint with forms created with Drupal 7 Webforms module using curl.

## Instructions

### Installation
Place the files into the modules folder as you would for any Drupal module. Since this module is not hosted by Drupal, you will need to manually update when necessary.

### Operation
The module only captures the values listed below. To captures these values, set the Key of the form fields fields in the Webform to the following (You've Got Leads field name - Key):

* PrimaryContact FirstName - FirstName
* PrimaryContact LastName - LastName
* PrimaryContact Address Address1 - Address1
* PrimaryContact Address City - City
* PrimaryContact Address State - State
* PrimaryContact Address Zip - Zip
* PrimaryContact Address Email - Email
* PrimaryContact Address PhoneHome - PhoneHome

A ProperityId field must also be included with the form.

* PropertyId - PropertyId

This is the target property for the form, and is needed in the construction of the endpoint URL. It is recommended that this be a hidden field type. Only one Property ID can be used at a time.

Important: ProperityId must be set in the form or the form will not be sent to You've Got Leads.

If the Key is not set in the form, it will not be included. There are no required fields by You've Got Leads, but this module does require a field named PropertyId.

## Note
This module should be considered minimally maintained, and is shared without guarantee or otherwise. It is hoped that sharing this here will be of some small benefit to your project.
