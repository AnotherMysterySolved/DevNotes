### _A work in progress..._
<br />
<br />
<br />
<br />
<br />


# HTML

<br />

## Block Level Elements
  *  p
  *  h1, h2, h3, h4, h5, h6
  *  ol, ul
  *  pre
  *  address
  *  blockquote
  *  dl
  *  div
  *  fieldset
  *  form
  *  hr
  *  noscript
  *  table
## Inline Elements
By default will not create a new line when rendered in the browser
**CANNOT** take width, height, margin, or padding styles
  *  a
  *  b
  *  big
  *  i
  *  small
  *  tt
  *  abbr
  *  acronym
  *  cite
  *  code
  *  dfn
  *  em
  *  kbd
  *  strong
  *  samp
  *  time
  *  var
  *  bdo
  *  br
  *  img
  *  map
  *  object
  *  q
  *  script
  *  span
  *  sub
  *  sup
  *  button
  *  input
  *  label
  *  select
  *  textarea

## Inline-Block Elements
Sit inline with the content but have the characteristics of a block element in that you **CAN** adjust width, height, margin, or padding styles
  *  Images
  *  Buttons
<br />

# JS
<br />

## FOR LOOPS
  ### Forward
```
    var vacationSpots = ['Paris', 'New York', 'Barcelona'];

    for (var i = 0; i < vacationSpots.length; i++) {
      console.log('I would love to visit ' + vacationSpots[i]);
    }
```

### Backward
```

   var vacationSpots = ['Paris', 'New York', 'Barcelona'];

    for (var i = vacationSpots.length - 1; i >= 0; i--) {
      console.log('I would love to visit ' + vacationSpots[i]);
    } 
```
    
## PUSH & POP - ARRAYS
```
  var bucketList = ['run', 'hike', 'swim'];

  bucketList.push('cycle', 'fish');
  bucketList.pop('run');

  console.log(bucketList);
```
## RANDOM NUMBER
  This will be between 0-100
```
  Math.floor(Math.random()*100)
```

## SUBSTRINGS
  "some word".substring(x, y) where x is where you start chopping and y is where you finish chopping the original string.
```
  "hello". substring(0, 2);
```

## SWITCH STATEMENTS
```
  var moonPhase = "full";

  switch (moonPhase) {
    case "full":
    	console.log("Howwwlll!!");
  		break;
    case "mostly full":
    	console.log("Arms and legs are getting hairier")
      break;
    case "mostly new":
      console.log("Back on two feet");
      break;
    default:
    	console.log('Invalid moon phase');
  		break;
  }
```

## WHILE STATEMENT
```
  var cards = ['Diamond', 'Spade', 'Heart', 'Club'];
  var currentCard = 'heart';

  while (currentCard !== 'Spade') {
    console.log(currentCard);

    var randomNumber = Math.floor(Math.random() * 4);

    currentCard = cards[randomNumber];
  }

  console.log('We got a spade!');
```
<br />

# jQuery
<br />


## HIDE AN ELEMENT(s)
```
function main() {
    $('.skillset').hide();
  }

  $(document).ready(main);
```

## FADE IN AN ELEMENT(s)
```
function main() {
    $('.skillset').hide();
    $('.skillset').fadeIn(1000);
  }

  $(document).ready(main);
```

## NEXT
  jQuery has a function named next to help us select elements that are next to another element. If we have this in our HTML:

```
  <div class='item-one'> ... </div>
  <div class='item-two'> ... </div>
  If we wanted to hide item-two, we could write:

  $('.item-one').next().hide();
```


## SHOW AN ELEMENT
  To show an element, the syntax looks as such:
```
  $('.example-class').show();
```
  show is attached directly to the jQuery selector.

  show will change the CSS attribute "display: none" to a visible display property, therefore showing the element.


## SLIDETOGGLE
jQuery provides a method named slideToggle that can animate an element's entrance and exit. The syntax looks like this:
```
$('.example-class').slideToggle(400);
```

## TEXT
  We can change the text of an element with the jQuery function text. It's syntax looks like this:
```
$('.my-selector').text('Hello world!');
```

## THIS
  $(this) selects the clicked element. If there are multiple elements with a class of .example-class, this will only toggle the class of the one that is clicked on.
```
  $('.example-class').on('click', function() {
    $(this).toggleClass('active');
  });
  ```

## TOGGLE
  toggle will hide or show an element, each time it is triggered. The syntax looks like this:
```
$('example-class').toggle();
```
## TOGGLECLASS
  We can toggle a CSS class with a jQuery function named toggleClass. The syntax looks like this:

  ```
  $('.example-class').toggleClass('active')
  ```
  
