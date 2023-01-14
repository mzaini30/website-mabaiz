# Columns

## Vertical alignment

```html
<div class="container text-center">
  <div class="row align-items-start">
    <div class="col">One of three columns</div>
    <div class="col">One of three columns</div>
    <div class="col">One of three columns</div>
  </div>
</div>
```

```html
<div class="container text-center">
  <div class="row align-items-center">
    <div class="col">One of three columns</div>
    <div class="col">One of three columns</div>
    <div class="col">One of three columns</div>
  </div>
</div>
```

```html
<div class="container text-center">
  <div class="row align-items-end">
    <div class="col">One of three columns</div>
    <div class="col">One of three columns</div>
    <div class="col">One of three columns</div>
  </div>
</div>
```

```html
<div class="container text-center">
  <div class="row">
    <div class="col align-self-start">One of three columns</div>
    <div class="col align-self-center">One of three columns</div>
    <div class="col align-self-end">One of three columns</div>
  </div>
</div>
```

## Horizontal alignment

```html
<div class="container text-center">
  <div class="row justify-content-start">
    <div class="col-4">One of two columns</div>
    <div class="col-4">One of two columns</div>
  </div>
  <div class="row justify-content-center">
    <div class="col-4">One of two columns</div>
    <div class="col-4">One of two columns</div>
  </div>
  <div class="row justify-content-end">
    <div class="col-4">One of two columns</div>
    <div class="col-4">One of two columns</div>
  </div>
  <div class="row justify-content-around">
    <div class="col-4">One of two columns</div>
    <div class="col-4">One of two columns</div>
  </div>
  <div class="row justify-content-between">
    <div class="col-4">One of two columns</div>
    <div class="col-4">One of two columns</div>
  </div>
  <div class="row justify-content-evenly">
    <div class="col-4">One of two columns</div>
    <div class="col-4">One of two columns</div>
  </div>
</div>
```

## Column wrapping

```html
<div class="container">
  <div class="row">
    <div class="col-9">.col-9</div>
    <div class="col-4">
      .col-4<br />Since 9 + 4 = 13 &gt; 12, this 4-column-wide div gets wrapped
      onto a new line as one contiguous unit.
    </div>
    <div class="col-6">
      .col-6<br />Subsequent columns continue along the new line.
    </div>
  </div>
</div>
```

## Column breaks

```html
<div class="container text-center">
  <div class="row">
    <div class="col-6 col-sm-3">.col-6 .col-sm-3</div>
    <div class="col-6 col-sm-3">.col-6 .col-sm-3</div>

    <!-- Force next columns to break to new line -->
    <div class="w-100"></div>

    <div class="col-6 col-sm-3">.col-6 .col-sm-3</div>
    <div class="col-6 col-sm-3">.col-6 .col-sm-3</div>
  </div>
</div>
```

```html
<div class="container text-center">
  <div class="row">
    <div class="col-6 col-sm-4">.col-6 .col-sm-4</div>
    <div class="col-6 col-sm-4">.col-6 .col-sm-4</div>

    <!-- Force next columns to break to new line at md breakpoint and up -->
    <div class="w-100 d-none d-md-block"></div>

    <div class="col-6 col-sm-4">.col-6 .col-sm-4</div>
    <div class="col-6 col-sm-4">.col-6 .col-sm-4</div>
  </div>
</div>
```

## Order classes

```html
<div class="container text-center">
  <div class="row">
    <div class="col">First in DOM, no order applied</div>
    <div class="col order-5">Second in DOM, with a larger order</div>
    <div class="col order-1">Third in DOM, with an order of 1</div>
  </div>
</div>
```

```html
<div class="container text-center">
  <div class="row">
    <div class="col order-last">First in DOM, ordered last</div>
    <div class="col">Second in DOM, unordered</div>
    <div class="col order-first">Third in DOM, ordered first</div>
  </div>
</div>
```

## Offset classes

```html
<div class="container text-center">
  <div class="row">
    <div class="col-md-4">.col-md-4</div>
    <div class="col-md-4 offset-md-4">.col-md-4 .offset-md-4</div>
  </div>
  <div class="row">
    <div class="col-md-3 offset-md-3">.col-md-3 .offset-md-3</div>
    <div class="col-md-3 offset-md-3">.col-md-3 .offset-md-3</div>
  </div>
  <div class="row">
    <div class="col-md-6 offset-md-3">.col-md-6 .offset-md-3</div>
  </div>
</div>
```

```html
<div class="container text-center">
  <div class="row">
    <div class="col-sm-5 col-md-6">.col-sm-5 .col-md-6</div>
    <div class="col-sm-5 offset-sm-2 col-md-6 offset-md-0">
      .col-sm-5 .offset-sm-2 .col-md-6 .offset-md-0
    </div>
  </div>
  <div class="row">
    <div class="col-sm-6 col-md-5 col-lg-6">.col-sm-6 .col-md-5 .col-lg-6</div>
    <div class="col-sm-6 col-md-5 offset-md-2 col-lg-6 offset-lg-0">
      .col-sm-6 .col-md-5 .offset-md-2 .col-lg-6 .offset-lg-0
    </div>
  </div>
</div>
```

## Margin utilities

```html
<div class="container text-center">
  <div class="row">
    <div class="col-md-4">.col-md-4</div>
    <div class="col-md-4 ms-auto">.col-md-4 .ms-auto</div>
  </div>
  <div class="row">
    <div class="col-md-3 ms-md-auto">.col-md-3 .ms-md-auto</div>
    <div class="col-md-3 ms-md-auto">.col-md-3 .ms-md-auto</div>
  </div>
  <div class="row">
    <div class="col-auto me-auto">.col-auto .me-auto</div>
    <div class="col-auto">.col-auto</div>
  </div>
</div>
```

## Standalone column classes

```html
<div class="col-3 p-3 mb-2">.col-3: width of 25%</div>

<div class="col-sm-9 p-3">.col-sm-9: width of 75% above sm breakpoint</div>
```

```html
<div class="clearfix">
  <img src="..." class="col-md-6 float-md-end mb-3 ms-md-3" alt="..." />

  <p>
    A paragraph of placeholder text. We're using it here to show the use of the
    clearfix class. We're adding quite a few meaningless phrases here to
    demonstrate how the columns interact here with the floated image.
  </p>

  <p>
    As you can see the paragraphs gracefully wrap around the floated image. Now
    imagine how this would look with some actual content in here, rather than
    just this boring placeholder text that goes on and on, but actually conveys
    no tangible information at. It simply takes up space and should not really
    be read.
  </p>

  <p>
    And yet, here you are, still persevering in reading this placeholder text,
    hoping for some more insights, or some hidden easter egg of content. A joke,
    perhaps. Unfortunately, there's none of that here.
  </p>
</div>
```
