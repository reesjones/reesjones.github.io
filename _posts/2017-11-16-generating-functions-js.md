---
title: JS generator functions in 15 seconds
layout: post
comments: true
---

Because concise example-based learning is most effective.

```
function *aGeneratorFunction() {
    console.log('stage 1');
    yield 123;
    console.log('stage 2');
    yield "almost there";
    console.log('stage 3, done');
    return {foo: "bar"};
}
```

Make a "Generator" object and run it:

```
let gen = aGeneratorFunction();
gen.next(); // {value: 123, done: false}
> stage 1
gen.next(); // {value: "almost there", done: false}
> stage 2
gen.next(); // {value: {foo: "bar"}, done: true}
> stage 3, done
```

Useful for writing more elegant code. Here are [some details](http://dmitrysoshnikov.com/ecmascript/javascript-the-core-2nd-edition/#execution-context) on how it works behind the scenes.
