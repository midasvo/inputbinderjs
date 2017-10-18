# inputbinderjs
Simple input binding to template text

### Usage

Include the .js file

`<script src='inputbinderjs.js'></script>`

Create an input field

`<input type="text" id="inputbindid" name="inputbind" value="intialvalue" />`

Instance the inputbinder

```
<script>
	var inputBinder = new inputBinder("inputbindid", ['div', 'p'], "#@initialinputtemplatetext@#", "dynamic-text-template");
</script>
```

The parameters are as follows:
	- InputID: "inputbindid" 
		- (used for getting the value out of the input field)
	
	- SearchTags: ['div', 'p'] 
		- (array of html tags that will be searched and replaced, helps targetting specific elements of the page) 
	
	- InitialTemplateText: "#@initialinputtemplatetext@#" 
		- (place this where you want the value to bind, will be replaced by a span with the class we can use)
	
	- TemplateClass: "dynamic-text-template" 
		- (target class for replacing)


#### Why

I made this script to easily, without JQuery, create input fields bound to template text. I like to create quick tutorials, and its easier to be able to customize the tutorial a bit while reading it (getting rid of 'example.tld' or '/path/to/your/dir' etc.).

##### License

Free. Feel free to use, customize, pull, fork, whatever. 