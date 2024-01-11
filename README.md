# At.js

### Just an idea, no code for the moment

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
<button @click="request:get:/test->#document">Click me bitch !</button>
```

### Multiple requests assign result to #document and #another-part (Sequencial version)
```html
<button @click="request:get:/test->#document,request:get:/test2->#another-part">Click me bitch !</button>
```

### Multiple requests assign results to #document and #another-part (Parralel version)
```html
<button @click="request:get:/test->#document|request:get:/test2->#another-part">Click me bitch !</button>
```

## Class

### Add class to a button on click
```html
<button @click="class:add:alert">Click me bitch !</button>
```

### Add class to another element on click
```html
<button @click="class:add:alert->#another-element">Click me bitch !</button>
```

### Toggle between two classes on a button
```html
<button @click="class:toggle:open,close">Click me bitch !</button>
```

### Remove class on #another-element
```html
<button @click="class:remove:open->#another-element">Click me bitch !</button>
```


