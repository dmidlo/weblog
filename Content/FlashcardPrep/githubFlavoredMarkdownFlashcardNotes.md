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
*by using the backslash character preceding the character that is to be escaped (not parsed by the markdown engine.)*

```markdown
this is an \<h1>
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
*By using an asterisk(\*), minus(\-), or plus (\+) along with a  space preceding the list item*

*__having groups of list symbols (\*, \-, and \+) will create seperate lists__*

```markdown
* list item dog
- list item phone number
* list item fourteen
+ list item pogo-stick
+ list item TheFallOfRome
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

# How do you create an ordered list in markdown?
*by using any number followed by a period `(.)` and a space*

```markdown
1. This
9. is
3. a
7. ordered
2. list
8. even
1. though
1. the numbers used
9. in markdown
4. are nonsensical
```

# How do you create an ordered sub-list in markdown?
*by applying indentation within an ordered list along with a sub-list character*
```markdown
1. This
9. is
3. a
    1. item 1
    44. item 2
    10. item 3
7. ordered
2. list
8. even
1. though
1. the numbers used
9. in markdown
4. are nonsensical
```

# How do you add a properly indented paragraph within a list in markdown?
*by following the indentation defined within the existing list along with line-breaks before and after the paragraph*

```markdown
1. This

    the quick brown fox jumped over the lazy dog.

9. is
3. a
    1. item 1
    
        Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s.
    
    44. item 2
    10. item 3
7. ordered
2. list
8. even
1. though
1. the numbers used
9. in markdown
4. are nonsensical
```

# How do you create an inline-style link with markdown?
*by using square brackets `[]` followed by parenthesis`()`.*

# How do you create an inline-style link with a title in markdown?

# How do you create a reference-style link using markdown?

# How do you create a relative reference link to a repository file in markdown

# 