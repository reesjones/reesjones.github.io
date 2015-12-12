---
layout: post
title: My first bash function
comments: true
---

I found a nice little [article](http://www.makeuseof.com/tag/4-ways-teach-terminal-commands-linux-si/) today on learning terminal commands in Linux. The first suggestion in the article was to echo a random command from the /bin directory every time an instance of bash starts up. I took their suggestion of wrapping the output in a cowsay speech bubble slightly further.

cowsay is a little program that prints text from standard input in a speech bubble coming from a cow (there are other animals/characters that you can specify). All I did was plop the cowsay command from the MakeUseOf article into a bash function called [cowtip](http://www.makeuseof.com/tag/4-ways-teach-terminal-commands-linux-si/) in my ~/.bashrc and ran it every time a terminal window is started. Here’s the code:

CowTip of the day!

```
function cowtip {
   cowsay -f $(ls /usr/share/cowsay/cows | shuf -n 1 | cut    -d -f1) $(whatis $(ls /bin) 2>/dev /null | shuf -n 1)
}
cowtip
```
Just put it in your `~/.bashrc` and it’ll spit out a random command and its description every time you start the terminal or run cowtip!

```
 ___________________________________
< dir (1) - list directory contents >
 -----------------------------------
       \   ^__^
        \  (oo)\_______
           (__)\       )\/\
               ||----W |
               ||     ||
```
