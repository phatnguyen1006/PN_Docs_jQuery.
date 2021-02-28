# PN_Docs_jQuery.

## List:

1. [jQuery](#jquery)
2. [Selector](#selector)
3. [AddClass](#addclass)
4. [RemoveClass()](#removeclass)
5. [ChangeCSS](#changeCss)
6. [ChangeHTML](#changeHTML)
7. [ChangeProp](#changeProp)
8. [Remove](#remove)
9. [Move](#move)
10. [Parent](#parent)
11. [Children](#children)
12. [Target A Specific Child](#target-a-specific-child)
13. [Target Even Elements](#target-even-element)
14. [Last](#last)

## jQuery

jQuery is one of the most widely used JavaScript libraries in the world.

In 2006 when it was released, all major browsers handled JavaScript slightly differently. jQuery simplified the process of writing client-side JavaScript, and also ensured that your code worked the same way in all browsers.

In this course, you'll learn how to use jQuery to select, remove, clone, and modify different elements on the page.

```html
<script>
  $(document).ready(function() {
    // add Command...
  }); 
</srcipt>
```

## Selector

When we want to adjust a selector:
- element:  $("element"). // $("button").
- class:    $(".class").  // $(".class-name").
- id:       $("#id").      // $("#id-name").  

## AddClass

We wanna add class "animated bounce" to a selector.

```javascript

  $(document).addClass("animated bounce");
  
```

## RemoveClass

We also can remove class "animated bounce" to a selector.

```javascript

  $(document).removeClass("animated-default");
  
```

## ChangeCSS

With a CSS:
When I need change the "color" is "red":

```javascript

  $(document).css("color","red");
  
```

## ChangeHTML

Another:
HTML

```javascript

  $("selector").html("<h2>Contents</h2>");
  
```

or we can change contents inside a tag element.
```javascript

  $("selector").text("contents");
  
```

## ChangeProp

Example:
```javascript

  $("selector").prop("disabled", true);
  
```

## Remove

Now let's remove an HTML element from your page using jQuery.

```javascript
  
  $("selector").remove()

```
  
## Move

### Just Move 
jQuery has a function called appendTo() that allows you to select HTML elements and append them to another element.

For examples, we wanna move "#target" from "#left" to "#right".  ...// "#left" and "#right" is "<div>" tags element.
  
```javascript
  
  $("#target").appendTo("#right");

```
### Clone and Move
In addition to moving elements, you can also copy them from one place to another.

jQuery has a function called clone() that makes a copy of an element.

For example, if we wanted to copy "#target" from our "#left" to our "#right", we would use:

```javascript
  
  $("#target").clone().appendTo("#right")

```

## Parent

Every HTML element has a parent element from which it inherits properties.

jQuery has a function called parent() that allows you to access the parent of whichever element you've selected.

```javascript

  $("target").parent().css("background-color","blue");

```

## Children

Of courses!
jQuery has a function called children() that allows you to access the children of whichever element you've selected.

```javascript

  $("target").children().css("color","red");

```

## Target a Specific Child

You've seen why id attributes are so convenient for targeting with jQuery selectors. But you won't always have such neat ids to work with.

Fortunately, jQuery has some other tricks for targeting the right elements.

jQuery uses CSS Selectors to target elements. The target:nth-child(n) CSS selector allows you to select all the nth elements with the target class or element type.

```javascript

  $(".target:nth-child(2)").addClass("animated bounce");

```

## Target Even Elements

You can also target elements based on their positions using :odd or :even selectors.

Note that jQuery is zero-indexed which means the first element in a selection has a position of 0. This can be a little confusing as, counter-intuitively, :odd selects the second element (position 1), fourth element (position 3), and so on.

Here's how you would target all the odd elements with class target and give them classes:

```javascript

  $(".target:odd").addClass("animated shake");

```

## Last

We're done playing with our jQuery playground. Let's tear it down!

jQuery can target the body element as well.

Here's how we would make the entire body fade out: 

```javascript
$("body").addClass("animated fadeOut");
```

But let's do something more dramatic. Add the classes animated and hinge to your body element.

```javascript

  $("body").addClass("animated hinge");

```
