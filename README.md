# mollie-form-field
Drupal module that offers a form field handling Mollie payments.

# Installation
This section describes how to install the module and get it working.

(Please note you need Libraries in order to use the GatherContent module)

1. Upload contents of the mollie-form-field folder to /sites/all/modules/contrib/mollie-form-field/ directory.
2. Download the Mollie Api for PHP at https://github.com/mollie/mollie-api-php
3. Transfer the contents of the Mollie Api for PHP to /sites/all/libraries/mollie-api-php/ directory (assuming you have already installed the Libraries module).
4. Install the Mollie Form Field module through the 'Modules' menu in Drupal
5. Click on the menu item "Configuration" and then click "Web Services > Mollie Field"
6. Insert your Mollie API Key

# How to use
This setion describes how to use the mollie form field.

1. Create a content-type of an entity-form
2. Add a field of the 'Mollie field' type with the 'Mollie widget'.
3. Under 'Field settings', configure how you want to use this field. For example, you can choose wether you want to use a specified amount the user has to pay, or give the user the option to specify the quantity of the transaction by himself.
4. Fill in the redirect path. This is the path the user will be redirected to, after making a payment (Take note that it's possible to use tokens in this field, assuming you have the Token API installed).
5. Fill in a payment description.
