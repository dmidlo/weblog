# How do make headers in markdown?
*By preceding the text with an octothorpe symbol (#) along with a space*

```markdown
# This is an h1
## This is an h2
###### This is an h6
```

# What is an alternative way to make headers in markdown?
*By leveraging an underlining style using hyphens `(----)`` or equals signs `(======) in the line following the header content.*

__*This is limited to `<h1>` and `<h2>`*__

```markdown
Alternative H1 Markdown Syntax
==============================

Alternative H2 Markdown Syntax
------------------------------
```

# How do you escape a character in markdown?
*by using the backslash character following the character that is to be escaped (not parsed by the markdown engine.)*

```markdown
this is an <\h1>
```

# How do you place emphasis using italics in markdown?
*by wrapping content using a set of single asterisks or underscores*

```Markdown
*This text will be emphasized with italics*
_This text will also be emphasized with italics_
```

# How do you place strong emphasis using bold in markdown?
*by wrapping content using a set of double asterisks or underscores*

```Markdown
**This text will be emphasized with bold**
__This text will also be emphasized with bold__
```

# How do you combine emphasis (italics) and strong emphasis (bold) using markdown?
*by following standard html nesting practices*

```markdown
Combined emphasis using **bold and _italics_**
```

# How do you strikethrough text in markdown?
*by wrapping content using a set of double tildes (~\~)*

```markdown
stike text by wrapping content using a set of double ~~asterisks~~ tildes. (~~)
```

# How do you create an unordered list in markdown?
*By using an asterisk and space preceding the list*

```markdown
* list item dog
* list item phone number
* list item pogo-stick
```

# How do you create a unordered sub-list in markdown?
*by applying indentation within an unordered list*

```markdown
* list item dog
    * list item dogName
    * list item dogFood
    * list item dogWalk
* list item phone number
* list item pogo-stick
```

* list item dog
    * list item dogName
    * list item dogFood
    * list item dogWalk
* list item phone number
* list item pogo-stick

# How do you create an ordered list in markdown?