# \<wired-tooltip\>

Tooltip with text that appears on hover over an element. It will be centered to an anchor element specified in the 'for' attribute, or, if that doesn't exist, centered to the parent node containing it.

<!--
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="wired-tooltip.html">
    <style is="custom-style">
      .inline {
        display: inline-block;
      }
      .container {
        padding: 50px 0;
      }
      button {
        margin: 0 25px;
      }
    </style>
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<div class="container">
  <div class="inline">
    <button>Click me!</button>
    <wired-tooltip text="Below"></wired-tooltip>
  </div>
  <button id="btn">Click me!</button>
  <wired-tooltip position="top" for="btn" text="Above"></wired-tooltip>
  <button id="lb">Click me!</button>
  <wired-tooltip position="left" for="lb" text="Left"></wired-tooltip>
  <button id="rb">Click me!</button>
  <wired-tooltip position="right" for="rb" text="Right"></wired-tooltip>
</div>
```


## Styling tooltip

<!--
```
<custom-element-demo>
  <template>
    <script src="../webcomponentsjs/webcomponents-lite.js"></script>
    <link rel="import" href="wired-tooltip.html">
    <style is="custom-style">
      .inline {
        display: inline-block;
      }
      .container {
        padding: 50px 0;
      }
      button {
        margin: 0 25px;
      }
      .colored {
        --wired-tooltip-border-color: red;
        --wired-tooltip-background: rgba(200, 200, 0, 0.2);
        color: blue;
      }
    </style>
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<div class="container">
  <div class="inline">
    <button>Click me!</button>
    <wired-tooltip class="colored" text="Fancy tooltip"></wired-tooltip>
  </div>
</div>
```