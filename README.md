# myOwnLineShowMoreLess

Show More Less - jQuery - Very useful tiny tool. [Demo](https://siva7170.github.io/myOwnLineShowMoreLess/index.html)

## Getting Started

This is simple plugin developed using jQuery.

### Prerequisites

* Latest jQuery

* `showmoreless.min.js`

### Initialization

Use latest jQuery above the end head tag and place "showmoreless.min.js" above the end body tag.

```html
<html>
  <head>
    <script src="js/jquery-3.5.1.min.js" type="text/javascript"></script> <!-- Please update with latest jQuery -->
  </head>
  <body>
    <!-- Your page content -->
    <script src="js/showmoreless.min.js" type="text/javascript"></script>
  </body>
</html>
```


## Usage

Below code is sample for how to use it. Please see methods and its functionalities below sections.

```html
<html>
<head>
    <script src="js/jquery-3.5.1.min.js" type="text/javascript"></script> <!-- Please update with latest jQuery -->
</head>
<body>
    <div class="show-less-div">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Morbi porttitor, lorem eget sagittis accumsan, dui nisl dictum sapien, a gravida nulla augue sit amet tortor. Proin fermentum erat a lobortis fringilla. Quisque id venenatis magna, sed gravida nulla. Fusce euismod ligula sed mauris finibus auctor. Donec nec neque id urna rutrum rhoncus. Suspendisse vehicula ante sed dolor euismod, vitae laoreet lectus tincidunt. Phasellus tincidunt pellentesque volutpat. Praesent ut velit sit amet dui maximus bibendum quis porttitor lacus. Mauris justo lectus, ullamcorper sit amet sodales nec, cursus a turpis. Integer sed libero semper, facilisis neque ut, venenatis neque.
        <br/>
        <br/>
        Nam aliquet cursus auctor. Phasellus nec lorem sed nunc facilisis dictum. Nullam efficitur, orci et dignissim tincidunt, lectus neque ultricies lorem, nec gravida nisi diam nec quam. Nullam mollis maximus dolor. Integer in suscipit metus. Proin rutrum lorem non pretium vulputate. Nunc et iaculis enim, sed aliquet odio. Maecenas nec diam et ex ullamcorper sagittis. Integer hendrerit metus non magna scelerisque elementum. Phasellus auctor nunc nisi, vel consectetur odio viverra non. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Duis tincidunt mi odio, sit amet rhoncus libero dapibus a. Donec varius, erat at finibus laoreet, ipsum velit viverra ante, at interdum ligula arcu vel arcu. Nullam tristique dictum faucibus. Aenean venenatis ultricies leo ac varius.
        <br/>
        <br/>
        Donec id luctus metus, eu tristique sapien. Nam in pharetra nulla, id eleifend nunc. Aliquam varius elementum eros nec scelerisque. Aenean id dolor felis. Sed venenatis magna id velit imperdiet, vitae ultricies nunc lobortis. Sed sit amet rutrum ipsum, vitae efficitur dolor. Nunc vitae fringilla nibh, vestibulum auctor urna.
    </div>
    <script src="js/showmoreless.min.js" type="text/javascript"></script>
    <script>
        $(document).ready(function(e){
            $('.show-less-div').myOwnLineShowMoreLess({
                showLessLine:3,
                lessAtInitial:true,
                showLessText:'Read Less',
                showMoreText:'Read More',
                showLessAfterMore:true
            });
        });
    </script>
</body>
</html>
```

## Plugin parameters

### showLessLine

- Type: `Integer`
- Default: `1`

To set how many line(s) you want to show when plugin show less text

### lessAtInitial

- Type: `Boolean`
- Default: `true`

When page loads, we can set how we want to show text whether less or more

### showLessAfterMore

- Type: `Boolean`
- Default: `true`

If we expand text by clicking Show More, then we can control that we need to show Show Less option by this param. If it is false, then Show Less will not show after text expanded. 

Note: If we want to use this param with false, then we should use lessAtInitial:true together with this option.

### showLessText

- Type: `String`
- Default: `Show Less`

We can change the Show Less text with this param.

### showMoreText

- Type: `String`
- Default: `Show More`

We can change the Show More text with this param.
