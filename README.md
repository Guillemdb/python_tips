# Python Development Conventions

## Introduction

This guide documents development conventions for Python at InstaDeep. This document in based in the coding conventions
 used at [Source{d}](https://github.com/src-d/guide/blob/master/engineering/conventions-python.md).
 
## Code Style

1. Contributing to existing external projects - do not change the style.
2. Follow the [Python Style guide](https://docs.python-guide.org/writing/style/).
3. Use [PEP8](https://www.python.org/dev/peps/pep-0008/) with 99 char line length limit.
4. Class methods order: first public, then protected (`_`), then private (`__`)
5. Use double quotes `"`. When a string contains single or double quote characters, however, use the other one to avoid
 backslashes in the string.
6. Favor `format()` when printing variables inside a string.
7. Do not use single letter argument names; use X and Y only in Scikit-learn context.
9. Use [Sphinx style](https://devguide.python.org/documenting/#style-guide) for docstrings.
10. Format of TODO and FIXME: `# TODO(mygithubuser): blah-blah-blah`.
11. Add [Type hinting](https://docs.python.org/3/library/typing.html) when possible.
12. Use standard [argparse](https://docs.python.org/3/library/argparse.html) for CLI interactions.


## Useful tips

1. Using [PyCharm](https://www.jetbrains.com/pycharm/download/#section=linux) as an IDE will help you highlight the most
 common mistakes amd help you enforce PEP8.

2. **Each function should do only one thing**. If you find yourself writing a long function that does a lot of stuff, consider
splitting it into different functions.

3. **Give variables a meaningful name**. If names became too long, use abbreviations. This abbreviations should be explained
in comments when defining the variable for the first time.

4. Keep in mind that coding is creating abstractions that hide complexity. This means that you should be able to get an
idea of what a function does just by reading its documentation and the comments.  

5. **Avoid meaningless comments**. Assume the person who is reading your code already know how to code in python, and take
advantage of the syntax of the language to avoid using comments. For example, a comment is welcome when it can save you
reading several lines of code that do stuff which is difficult to understand. 

6. **Document the functions**, and make sure that it is easy to understand what all the parameters are. When working with tensors
and vectors, specify its dimensions when they are not obvious.

7. **Follow the [Zen of Python](https://www.python.org/dev/peps/pep-0020/)**, it is your best friend.

8. A well documented function lets you know what it does and how to use it without having to take a look at its code.
**Document all the functions**! It is a pain in the ass but it pays off.



## Example codebase

Reading well-written Python code is also a way to improve your skills. Please avoid copying anything that has been written
by a researcher; it will likely be a compendium of bad practices. Instead, take a look at any of the following projects:

- [TensorFlow](https://github.com/tensorflow/tensorflow)

- [Django](https://github.com/django/django)

- [Flask](https://github.com/pallets/flask)

- [Jinja 2](https://github.com/pallets/jinja)

When it comes to Reinforcement Learning, please avoid at any cost using OpenAI baselines as an example. Instead you can
take a look a [Intel Nervana's Coach](https://github.com/NervanaSystems/coach) 


## Resources

- **The Zen of Python in examples**: 
    - [Post in Medium](https://medium.com/@Pythonidaer/a-brief-analysis-of-the-zen-of-python-2bfd3b76edbf)
    - [Quora post](https://www.quora.com/What-do-different-aphorisms-in-The-Zen-of-Python-mean)
    - [Code example](https://gist.github.com/evandrix/2030615)
    
- **Idiomatic Python**:
    - Blog post about [Idiomatic Python](https://medium.com/the-andela-way/idiomatic-python-coding-the-smart-way-cc560fa5f1d6)    
    - [More Python Idioms](http://prooffreaderplus.blogspot.com/2014/11/top-10-python-idioms-i-wished-id.html)
