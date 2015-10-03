---
title: A tidbit of Java magic - integer caching
layout: post
---

I came across a code snippet on StackOverflow:

```
Integer a = 42;
Integer b = 42;
System.out.println(a == b);
Integer c = 555;
Integer d = 555;
System.out.println(c == d);
```

The first print statement prints `true` and the second one prints `false`.

Wait, what?

The second comparison makes sense. `==` in Java compares references to see if they
are the same object *in memory* (and primitives are compared by their literal value).
So `c == d` should return false, since they're not the same object in memory.
The `Object.equals()` method is a *functional* comparison, but it doesn't check
actual reference equality, e.g. it doesn't check the addresses of the reference variables.
So why does the first comparison equate to true?

The answer can be found in the Java Langauge Specification, [chapter 5](http://docs.oracle.com/javase/specs/jls/se7/html/jls-5.html#jls-5.1.7).
Two primitives being autoboxed into references via a boxing conversion may qualify to
be cached for optimization purposes. Caching the more commonly used primitive values
leads to faster access time, so these certain commonly used primitives are cached:

 * `true`, `false`
 * `byte` or `char` in the range `\u0000` to `\u007f`
 * `int` or `short` in the inclusive range of -128 to 127

So in the snippet above, `a == b` is true because `a` and `b` are between -128 and 127, so
when a new `Integer a = 42;` is created, it simply points to a previously cached Integer object.

Note that this only works when primitive `int`s are autoboxed to `Integer`s. If two `Integer`
objects are created (not autoboxed from the primitive type)...

```
Integer e = new Integer(4);
Integer f = new Integer(4);
System.out.println(e == f);
```

...then the comparison will be false, since both `Integer` references were explicitly initialized
as separate objects.

Interesting stuff!

