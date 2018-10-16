---
layout: post
comments: true
title:  Nomenclature Tips
date:   2018-06-23 07:07:00
---

This guide is designed to help you choose variable names, functions, parameters, and modules within your program.

Choosing a certain name can help when developing another or you look at your code in the future and it will be easier to understand. It will still avoid future code refactoring.

## Rules you should consider:

* Follow a pattern for the names and consistently follow this pattern. In [Elixir](http://elixir-lang.github.io) for example, by default, the names of the variables, functions and atoms must be lowercase and follow the `snake_case` style, for modules uses `CamelCase`, keeping acronym in capital letters, etc. Different languages follow different standards, it is up to you a good programmer, to follow the good practices of the language you are programming.

* Avoid abbreviations unless they are standardized and of good use.

* For variables and parameters, for the most part, the name must be sufficient to be descriptible.

* The name should describe the meaning of the data rather than its type. Example: `name` instead of `string`, unless this data is generic.

* Functions and modules may have names that express what they _do_ or _return_, but never in what _way_ do they do - because how it's done can change (Example: use another library to do the same task, use a more efficient method to solve a problem).

Some examples:

```elixir
def tran(a, b) do

def remove_and_add(a, b) do

def transfer(withdrawal_account, deposited_account) do
```

All 3 functions transfer from one account to another.

The first example is not good, because it is not clear if the function transforms something or transfers, because it is abbreviated and its parameters do not indicate what they refer. The second is also unclear, the function name speaks what it does, but it is out of context to know what it takes and where it adds. The third one is great, clear and easy to understand, because the name of the function tells what it does and its parameters clearly demonstrate what is expected.

### Recommendation

Use an editor that has auto-complete (or install a plugin in the editor you use), so you do not have to write a variable that has a big name at all times

#### Bibliography

[- Programming in Python 3: A Complete Introduction to the Python Language](http://www.informit.com/store/programming-in-python-3-a-complete-introduction-to-9780321680563)

[- Elixir Style Guide](https://github.com/christopheradams/elixir_style_guide/blob/master/README.md)