---
author:
  name: John Doe
  twitter: johndoetwitter
  picture: /images/johndoe.png
---

Any file that contains a YAML front matter block will be processed by Jekyll as a special file. The front matter must be the first thing in the file and must take the form of valid YAML set between triple-dashed lines. Here is a basic example:

---
layout: post
title: Blogging Like a Hacker
---
Between these triple-dashed lines, you can set predefined variables (see below for a reference) or even create custom ones of your own. These variables will then be available for you to access using Liquid tags both further down in the file and also in any layouts or includes that the page or post in question relies on.

UTF-8 Character Encoding Warning
If you use UTF-8 encoding, make sure that no BOM header characters exist in your files or very, very bad things will happen to Jekyll. This is especially relevant if you’re running Jekyll on Windows.

Front Matter Variables Are Optional
If you want to use Liquid tags and variables but don’t need anything in your front matter, just leave it empty! The set of triple-dashed lines with nothing in between will still get Jekyll to process your file. (This is useful for things like CSS and RSS feeds!)
