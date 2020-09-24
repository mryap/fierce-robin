---
title: "Take full advantage of these 10 Python3 features "
date: 2020-09-24T17:07:05.192Z
excerpt: Here are 10 Python 3 features that will change the way you are writing
  code today.
template: post
---
1. Enumerations
2. Data classes
3. Pathlib
4. Type hints
5. F-strings
6. Extended iterable unpacking
7. Walrus operator
8. async IO
9. Underscore in numeric literals
   10.LRU cache

<!--StartFragment-->

1. Enumerations 

Python 3.4+ Instead of cluttering your code with constants, you can create an enumeration using the Enum class. An enumeration is a set of symbolic names bound to unique, constant values.

3. Pathlib

THis is my favourite! pathlib solves a pet peeve of mine. The pathlib module provides a way to interact with the file system in a much more convenient way than dealing with os.path or the glob module. The pathlib module makes everything simpler.  

You can join paths by '/' operator:

<!--StartFragment-->



```
data_folder = Path("my_project/data/")
file_to_open = data_folder/"raw_data.txt"
```

<!--EndFragment-->

Moreover, you can directly get a content of the file, for example

```
print(file_to_open.read_text())
```

[More info on Pathlib](https://medium.com/@ageitgey/python-3-quick-tip-the-easy-way-to-deal-with-file-paths-on-windows-mac-and-linux-11a072b58d5f)

<!--StartFragment-->

4. Type hints  

You can use type hints to indicate the type of a value in your code. For example, you can use it to annotate the arguments of a function and its return type. These hints make your code more readable, and help tools understand it better.

![](/images/screenshot_2020-09-24-santiago-on-twitter.png)

<!--EndFragment-->

5. f-strings 

Instead of having to use the \`.format()\` method to print your strings, you can use f-strings for a much more convenient way to replace values in your strings. f-strings are much more readable, concise, and easier to maintain.

6. Underscores in Numeric Literals  

This one is a small, nice addition: you can use underscores in numeric literals for improved readability. This will shave off a few seconds every time you had to count how many digits a number had.

<!--EndFragment-->