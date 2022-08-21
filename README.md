## vim-indent-object

<!-- vim-markdown-toc GFM -->

- [Intro](#intro)
- [Install](#install)
- [Usage](#usage)
- [FeedBack](#feedback)

<!-- vim-markdown-toc -->

### Intro

Vim text objects
provide a convenient way to select and
operate on various types of objects.

These objects include regions surrounded by
    various types of brackets and
    various parts of language (ie sentences,  paragraphs,  etc). 

This plugin defines a new text object,
based on  indentation levels.
This is very useful in languages such as Python,
 

### Install

- vim-plug

```vim
Plug 'michaeljsmith/vim-indent-object'
```

### Usage

This plugin defines two new text objects.


| Key bindings | Description                                                 |
| ------------ | ----------------------------------------------------------- |
| `<count>ai`  | **A**n **I**ndentation level and line above.                |
| `<count>ii`  | **I**nner **I**ndentation level (**no line above**).        |

| `<count>aI`  |                              and lines above/below.         |
| `<count>iI`  |  same as ii                                                     |


Just like regular text objects,
these mappings can be used either with operators expecting a motion,
    such as `d` or `c`,
as well as in visual mode.


In visual mode the mapping can be repeated,
    which has the effect of iteratively increasing the scope of indentation block selected.
Specifying a count can be used to
achieve the same effect.


