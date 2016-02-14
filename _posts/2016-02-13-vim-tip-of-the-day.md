---
title: Vim tip&#58; view file state from a certain amount of time ago
layout: post
---

I found a nice little productivity hack in vim:

```
:earlier 30m
```

This resets the file currently being edited to the state it was in 30 minutes ago.
Cool! You can also use ```:earlier 30s``` for 30 seconds ago, and ```:earlier 30h``` 
for 30 hours ago.

```:later``` or ```:later 30m``` will reset the file back to the latest state.

Also: if you're itching to go home early from work, just open the files you're working 
on for the day and try ```:later 8h```
