@page index jQuery dForm

# jQuery dForm

The jQuery.dForm plugin allows you to create your HTML forms programmatically from JavaScript objects 
(and therefore JSON, too).

Usage:

	var formdata =
	{
		"action" : "index.html",
		"method" : "get",
		"elements" : 
		[
			{
				"name" : "textfield",
				"caption" : "Label for textfield",
				"type" : "text",
				"value" : "Hello world"
			},
			{
				"type" : "submit",
				"value" : "Submit"
			}
		]			
	};
	$("#myform").buildForm(formdata);
	
	// Or to load the form definition via AJAX
	$("#myform").buildForm("http://example.com/myform.json");


## How to get it:

[Download](http://github.com/downloads/daffl/jquery.dform/jquery.dform-0.1.4.tar.gz) the latest package (0.1.4(

Clone the current master on [GitHub](http://github.com/daffl/jquery.dform/)


## How to get involved:

* Visit the [jQuery.dForm Google Group](http://groups.google.com/group/jquery-dform)
* Fork the project on [GitHub](http://github.com/daffl/jquery.dform/)
* Follow [@daffl](http://twitter.com/daffl) on Twitter


## What it is for:

There are many server side web frameworks that support HTML form generation,
but you often end up mixing client (e.g. JavaScript validation) and server side processing concerns together.

This plugin moves the generation of forms entirely on the client side so that the server just has to provide a 
JavaScript object (usually as JSON) that contains all the information needed to create this form.
It is easily extensible for custom form elements and properties.


## You should try this plugin if you want to

* manage all your form related jQuery plugins in a unified way (jQuery UI and the Validation plugin
supported out of the box)
* scaffold forms from business objects of your server side framework
* have an easy way to include jQuery UI elements and JavaScript validation
* write JavaScript instead of HTML markup since your page doesn't run without JS anyway
