# At.js

## Attributes
- @click
- @doubleclick
- @change
- @mousemove
- @mouseover
- @mouseout

## Request
### Simple request, assign result to #document
```html
<button @click="request:get:/test->#document">
```

### Multiple requests assign result to #document and #another-part (Sequencial version)
```html
<button @click="request:get:/test->#document,request:get:/test2->#another-part">
```

### Multiple requests assign results to #document and #another-part (Parralel version)
```html
<button @click="request:get:/test->#document|request:get:/test2->#another-part">
```

## Class

### Add class to a button on click
```html
<button @click="class:add:alert">
```

### Add class to another element on click
```html
<button @click="class:add:alert->#another-element">
```
