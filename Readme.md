### CDN
Available on [jsdelivr](https://cdn.jsdelivr.net/npm/vue-resource@1.3.5), [unpkg](https://unpkg.com/vue-resource@1.3.5) or [cdnjs](https://cdnjs.com/libraries/vue-resource).
```html
<script src="https://cdn.jsdelivr.net/npm/vue-resource@1.3.5"></script>
```

# Hide Function
### Hides an element if it was visible
```js
$( ".target" ).hide();
```

# Show Function
### Shows an element if it was hidden
```js
$( ".target" ).show();
```

# Show Function
### Shows an element if it was hidden
```js
$( ".target" ).show();
```

# html Function
### Gets or sets an inner HTML of an element
```js
$( "div.demo-container" ).html();
```

# append Function
### Injects an element into the DOM after the selected element
```js
$( ".inner" ).append( "<p>Test</p>" );
```

# prepend Function
### Injects an element into the DOM before the selected element
```js
$( ".inner" ).prepend( "<p>Test</p>" );
```

# on Function
### Attaches an event listener to an element
```js
$( "#dataTable tbody tr" ).on( "click", function() {
  console.log( $( this ).text() );
});
```

# off Function
### Detaches an event listener from an element
```js
// ... Now foo will be called when paragraphs are clicked ...
$( "body" ).on( "click", "p", foo );
 
// ... Foo will no longer be called.
$( "body" ).off( "click", "p", foo );
});
```


# css Function
### Gets or sets the style attribute value of an element
```js
$( '.div' ).css( "background-color",'white' );
```

# attr Function
### Gets or sets any attribute of an element
```js
var title = $( "div" ).attr( "title" );
});
```

# val Function
### Gets or sets the value attribute of an element
```js
$( "select#foo" ).val();
});
```

# text Function
### Gets the combined text of an element and its children
```js
$( "div.demo-container" ).text()
```

# each Function
### Iterates over a set of matched elements
```html
<ul>
  <li>foo</li>
  <li>bar</li>
</ul>
```
```js
$( "li" ).each(function( index ) {
  console.log( index + ": " + $( this ).text() );
});
```
### Result
```html
 0: foo
1: bar 
```
