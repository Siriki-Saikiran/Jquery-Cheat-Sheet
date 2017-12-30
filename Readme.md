
# hide 
### Hides an element if it was visible
```js
$( ".target" ).hide();
```

# show 
### Shows an element if it was hidden
```js
$( ".target" ).show();
```

# html 
### Gets or sets an inner HTML of an element
```js
$( "div.demo-container" ).html();
```

# append 
### Injects an element into the DOM after the selected element
```js
$( ".inner" ).append( "<p>Test</p>" );
```

# prepend 
### Injects an element into the DOM before the selected element
```js
$( ".inner" ).prepend( "<p>Test</p>" );
```

# on 
### Attaches an event listener to an element
```js
$( "#dataTable tbody tr" ).on( "click", function() {
  console.log( $( this ).text() );
});
```

# off 
### Detaches an event listener from an element
```js
// ... Now foo will be called when paragraphs are clicked ...
$( "body" ).on( "click", "p", foo );
 
// ... Foo will no longer be called.
$( "body" ).off( "click", "p", foo );
});
```


# css 
### Gets or sets the style attribute value of an element
```js
$( '.div' ).css( "background-color",'white' );
```

# attr 
### Gets or sets any attribute of an element
```js
var title = $( "div" ).attr( "title" );
});
```

# val 
### Gets or sets the value attribute of an element
```js
$( "select#foo" ).val();
});
```

# text 
### Gets the combined text of an element and its children
```js
$( "div.demo-container" ).text()
```

# each 
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

# find 
### Gets or sets the value attribute of an element

```html
<ul class="level-1">
  <li class="item-i">I</li>
  <li class="item-ii">II
    <ul class="level-2">
      <li class="item-a">A</li>
      <li class="item-b">B
        <ul class="level-3">
          <li class="item-1">1</li>
          <li class="item-2">2</li>
          <li class="item-3">3</li>
        </ul>
      </li>
      <li class="item-c">C</li>
    </ul>
  </li>
  <li class="item-iii">III</li>
</ul>

If we begin at item II, we can find list items within it: 
```
```js
$( "li.item-ii" ).find( "li" ).css( "background-color", "red" );
```
```html
The result of this call is a red background on items A, B, 1, 2, 3, and C. Even though item II matches the selector expression, it is not included in the results; only descendants are considered candidates for the match.
```
