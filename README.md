# Custom DropDown 
Custom dropdown with Javascript &amp; jquery

Include the jQuery library and the custom-dropdown.js + custom-dropdown.css files  in your index.html file.

Create a DIV with an id which contains a wrapper, a (hidden) drop-down list and a “label” which we will wrap into a span. 

```html
<div class="dropdown-container">
    <div id="dd" class="wrapper-dropdown" tabindex="1">
        <span>John Doe</span>
        <ul class="dropdown">
            <li><a href="#"><i class="icon-user"></i>Profile</a></li>
            <li><a href="#"><i class="icon-cog"></i>Settings</a></li>
            <li><a href="#"><i class="icon-remove"></i>Log out</a></li>
        </ul>
    </div>
</div>
```

Build the dropdown by running the plugin on page load
```
 $(function() {
	var dd = new DropDown( 
		$('#dd'),     		// element
		'absolute', 		// element position
		'220px',     		// element width
		'#d7dadd',  		// Dropdown header Background colour
		‘#000000' , 		// Dropdown header text colour
		'#3e3e3e',		// Dropdown after selection header Background colour
 		'#ffffff',		// Dropdown after selection header text colour
		'#a4a4a5',		// Dropdown options background colour
		'#ffffff		// Dropdown options text colour
	);
  });
```
