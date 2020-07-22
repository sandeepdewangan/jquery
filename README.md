# jQuery 

## Basics
* Open up browser and type `jQuery` in console to check jQuery imported.
* With `$` we can select any thing.

eg. \
`$("img")` -> selects all image tags\
`$(".sale")` -> selects all elements with class sale\
`$("#bonus")` -> selects element with id bonus\
`$("li a")` -> selects all tag inside li\


## Examples

### Basic Examples

```html
<h1>jQuery Tutorial</h1>

    <h3>To Buy</h3>
    <ol>
        <li>Cheese</li>
        <li>Sause <a href="#">Goto</a></li>
        <li id="good">Red Chilli</li>
    </ol>
```

### Query

|# | Query | Output|
|---|---|---|
|1 | `$("h1")[0]` | `<h1>jQuery Tutorial</h1>`|
|2 | `$("a")[0]`| `<a href=​"#">​Goto​</a>​`|
|3 | `$("li a")[0]`| `<a href=​"#">​Goto​</a>​`|
|4 | `$("#good")[0]`| `<li id=​"good">​Red Chilli​</li>​`|

### Functions

#### Example 1: CSS Property
`$("h1").css('color','red')` - H1 tag becomes red color

#### Example 2: Changes h1 tag color and weight. (Method 1)
```js
<script>
    var styles = {
      color : "pink",
      fontWeight : "bold"
    };
    $("h1").css(styles);
</script>
```

#### Example 3: Changes h1 tag color and weight. (Method 2)
```js
<script>
    $("h1").css({color: "red", fontWeight: "bold"});
</script>
```

## jQuery Methods
```html
<!doctype html>
<html lang="en">
  <body>
    <h1>jQuery Methods</h1>

    <input type="text" placeholder="Enter something">

    <select>
      <option>Raipur</option>
      <option>Jaipur</option>
      <option>Kanpur</option>
    </select>

    <ul>
      <li> Item 1 </li>
      <li> Item 2 </li>
      <li> Item 3 </li>
    </ul>

    <script src="https://code.jquery.com/jquery-3.5.1.min.js" integrity="sha256-9/aliU8dGd2tb6OSsuzixeV4y/faTqgFtohetphbbj0=" crossorigin="anonymous"></script>
  </body>
</html>
```

#### Examples
* `$('h1').text('New Text')` - Selects h1 tag and edit text as 'New Text'.
* `$('h1').text()` - Gets the text of h1 tag.
* `$('ul').html()` - Gets the html of ul tag. 
    ```html
    <li> Item 1 </li>
    <li> Item 2 </li>
    <li> Item 3 </li>
    ```
* `$('ul').html("<li>New Item 1</li> <li>New Item 2</li>")` - Update ul tag elements
    ```html
    New Item 1
    New Item 2
    ```
* `$('input').val()` - graps the input box entered text
* `$('input').val('sandeep dewangan')` - put the text into input box
* `$('select').val()` - graps the select box selected text

