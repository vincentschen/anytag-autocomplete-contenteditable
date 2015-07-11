#Any-Tag Autocomplete for Contenteditable 

This is a bootstrap plugin to autocomplete tags for contenteditable div elements. Allows user to set any string as the inline tag to prompt autocomplete. 

##Requirements 
- bootstrap-typeahead.js
- caret-position.js
- jquery.js 
- rangy-core.js 

```html
<!-- Dependencies --> 
<script src="deps/jquery.js"></script>
<script src="deps/bootstrap-typeahead.js"></script>
<script src="deps/rangy-core.js"></script>
<script src="deps/caret-position.js"></script>

<script src="bootstrap-tagautocomplete.js"></script>
```

##Usage 

Attach handler to desired div and pass options. 

####Options 
- **tag** (required _string_): autocomplete will be triggered by this tag 
- **source** (required _array_): filters results from source 
- **suffix** (optional _string_): appends suffix upon selection

#####Original Options work as well 
- **after** (optional _function_): to run after selection  
- From bootstrap-typeahead: **items**, **updater**, **matcher**, **highlighter** and **sorter**.

```javascript
//initialize div element 
<div id="example" contenteditable="true"></div>

//apply handler 
$('div#example').tagautocomplete({
    tag: '##',
    source: ['ann', 'bill', 'casey'], 
    suffix: "## "
});
```

##Contributing
Originally Forked from <a href="https://github.com/Sandglaz/bootstrap-tagautocomplete/">Sandglaz</a>. 
