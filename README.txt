Module: Omniture Integration
Author: Greg Knaddison http://knaddison.com
Based on Google Analytics module by Mike Carter <www.ixis.co.uk/contact>


Description
===========
Adds the Omniture statistics system to your website.

Requirements
============

* Omnitureuser account


Installation
============
* Copy the 'omniture' module directory in to your Drupal
modules directory as usual.

Customization
============
* You can customize the module to your site to create variables
more suited to tracking your needs by 
1) creating a php file called omniture.inc in the same directory
as the omniture.module file
2) Creating a function in that file called omniture_variables which should 
return an array of variables with the following structure/use:

       $omniture_variables['s.pageName'] => "This is my page name";

Will be converted to the JavaScript 

     var s.pageName="This is my page name";


Usage
=====
You will also need to define what user roles should be tracked.
Simply tick the roles you would like to monitor.

You can also add JavaScript code in the "Advanced" section of the settings.

All pages will now have the required JavaScript added to the
HTML footer can confirm this by viewing the page source from
your browser.

'admin/' pages are automatically ignored by this module.


$Id$
