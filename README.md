# Phxsolution Formbuilder

**Extension for Magento 1**

Tested for Magento 1.9.3.1

Module version 0.3.2

---

*Please note that we are not the developer of this extension. In this repository, we only added modman and composer support. We will not provide any support for this repository. If you have any problems on integration, please use the official link provided above.*

## Overview

With this module, administrators can create custom forms that are shown in the frontend.

For more information, please visit https://www.magentocommerce.com/magento-connect/custom-formbuilder.html.

## Installation

Add the `require` and `repositories` sections to your composer.json as shown below and run `composer update`

```
{
    ...
    
    "repositories": [
    
        ...
        
        {"type": "git", "url": "https://github.com/kirchbergerknorr/magento1_phxsolution_formbuilder"},
        
        ...
    ],
	
    ...
	
    "require": {
        
        ...
        
        "kirchbergerknorr/magento1_phxsolution_formbuilder": "^0.3.2",
        
        ...
    },
    
    ...
}
```

## Usage

Add the following code to a CMS page or block to display a form created in the administrator panel

```
{{block type="formbuilder/frontend_form" name="frontend_form" form_id="[ID of your form]" template="formbuilder/form.phtml"}}
```