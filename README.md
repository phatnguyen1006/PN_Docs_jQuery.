# PN_Docs_jQuery.

## List:

1. [jQuery](#jquery)
2. [Selector](#selector)
3. [AddClass](#addclass)
4. [RemoveClass()](#removeclass)
5. [ChangeCSS](#changeCss)
6. [ChangeHTML](#changeHTML)
7. [ChangeProp](#changeProp)

## jQuery

jQuery is one of the most widely used JavaScript libraries in the world.

In 2006 when it was released, all major browsers handled JavaScript slightly differently. jQuery simplified the process of writing client-side JavaScript, and also ensured that your code worked the same way in all browsers.

In this course, you'll learn how to use jQuery to select, remove, clone, and modify different elements on the page.

```html
<script>
  $(document).ready(function() {
    
  })
</srcipt>
```

## Selector

When we want to adjust a selector:
- element:  $("element"). // $("button").
- class:    $(".class").  // $(".class-name").
- id:       $("id").      // $("id-name").  

## AddClass

We wanna add class "animated bounce" to a selector.

```html

  $(document).addClass("animated bounce");
  
```

## RemoveClass

We also can remove class "animated bounce" to a selector.

```html

  $(document).removeClass("animated-default");
  
```

## ChangeCSS

With a CSS:
When I need change the "color" is "red":

```html

  $(document).css("color","red");
  
```

## ChangeHTML

Another:
HTML

```html

  $("selector").html("<h2>Contents</h2>");
  
```

or we can change contents inside a tag element.
```html

  $("selector").text("contents");
  
```

## ChangeProp

Example:
```html

  $("selector").prop("disabled", true);
  
```
