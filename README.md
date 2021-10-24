# be-slotful

Emulate (bare-bones) slots without the benefit of Shadow DOM.

Used in conjunction with be-referential

```html
<template be-definitive='{
    "config": {
        "tagName": "my-custom-element",
        "propDefaults":{
            "noshadow": true
        }
    }
}'>
  <div be-slotful='{
      "ref": "my-ref"
  }'>
</template>

<my-custom-element>
    <template be-referential='{
        "ref": "my-ref"
    }'>
        <my-content></my-content>
    </template>
</my-custom-element>
```