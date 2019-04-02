![github logo](https://upload.wikimedia.org/wikipedia/commons/thumb/2/29/GitHub_logo_2013.svg/320px-GitHub_logo_2013.svg.png)
![Markdown logo](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/208px-Markdown-mark.svg.png)

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
*by using square brackets `[]` followed by parenthesis`()` using the following syntax:*

__*`[link name](url)`*__

```markdown
[A link to search for answers](https://www.google.com)
```

# How do you create an inline-style link with a hover-over title in markdown?
*by adding double-quotes `""` to the url portion of the standard markdown link syntax.*

__*`[link name](url "hover-over title")`*__

```markdown
[A link to search for answers](https://www.google.com "Google Search")
```

# How do you create a reference-style link using markdown?
*by using square brackets `[]` instead of parenthesis `()` as the second declaration in the standard markdown link syntax along with a bibliographic reference using square brackets `[]` and a colon `:`*


```markdown
[link-text][Arbitrary case-insensitive reference text]

[Arbitrary case-insensitive reference text]: referenceURL
```

__Example:__
```markdown
[The Dunning-Kruger effect][dunning, kruger]

[Negativity bias][1]

[Survivorship bias]


[dunning, kruger]: https://en.wikipedia.org/wiki/Dunning%E2%80%93Kruger_effect
[1]: https://en.wikipedia.org/wiki/Negativity_bias
[Survivorship bias]: https://en.wikipedia.org/wiki/Survivorship_bias
```
__*Feature: Bibilographic references are not displayed in-browser on github*__


*there is also a shorthand version using the link text found in the first set of square brackets*

```markdown
[link-text]

[link-text]: referenceURL
```
__*Feature: Bibilographic references are not displayed in-browser on github*__

# How do you create a relative reference link to a repository file in markdown
*by using dot-slash notation `./dir1/dir2/file.txt` in the paranthetical link definition using standard markdown link syntax*

__*`[Repository File](../dir1/dir2/file.txt)`*__

```markdown
[Inspectional Book Review Template](../ContentTemplates/InspectionalBookReviewTemplate.md)
```

__*you can likewise use the biblographic reference style to link to repository files*__

```markdown
[A workflow for gettting the most out of skim reading][Inspectional Book Review Template]

[Inspectional Book Review Template]: ../ContentTemplates/InspectionalBookReviewTemplate.md
```
__*Feature: Bibilographic references are not displayed in-browser on github*__

# How do you link to a Github Issue or Pull request using its RAW URL in markdown?
*by using the issue's RAW URL in the paranthetical link definition using standard markdown link syntax*

__*`[#1](https://github.com/user/repo/issues/1)`*__

```markdown
[#1](https://github.com/dmidlo/weblog/issues/1)
```

__*you can likewise use the biblographic reference style to link to repository files*__

```markdown
[Issue - How do you link to a Github Issue or Pull request in markdown?][#1]

[#1]: https://github.com/dmidlo/weblog/issues/1
```
__*Feature: Bibilographic references are not displayed in-browser on github*__

# How do you link to a git commit on github in markdown?
*by using the commits's RAW URL in the paranthetical link definition using standard markdown link syntax*

__*`[commit text](https://github.com/user/repo/commit/hash)`*__

```markdown
[this commit](https://github.com/dmidlo/weblog/commit/c54e55103c7e9f865e05a2f2217551ad052e32c4)

[c54e551](https://github.com/dmidlo/weblog/commit/c54e551)
```


__*you can likewise use the biblographic reference style to link to repository files*__

```markdown
[this commit][c54e551]

[c54e551]: https://github.com/dmidlo/weblog/commit/c54e551
```
__*Feature: Bibilographic references are not displayed in-browser on github*__

# How do you add an image link in-line using markdown?
*by using a exclaimation mark `!`, square brackets `[]`, followed by parenthesis`()` using the following syntax:*

__*`![alt text](image URL)`*__

```markdown
![Markdown logo](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Markdown-mark.svg/416px-Markdown-mark.svg.png)
```

# How do you add an image link using a bibliographic-style reference in markdown?
*by using an exclaimation mark `!`, and square brackets `[]` instead of parenthesis `()` as the second declaration in the standard markdown image link syntax along with a bibliographic reference using square brackets `[]` and a colon `:`*

```markdown
![alt text][Arbitrary case-insensitive reference text]

[Arbitrary case-insensitive reference text]: image URL
```

__Example:__
```markdown
![github logo][wikimedia github logo]


[wikimedia github logo]: https://upload.wikimedia.org/wikipedia/commons/thumb/2/29/GitHub_logo_2013.svg/320px-GitHub_logo_2013.svg.png

```
__*Feature: Bibilographic references are not displayed in-browser on github*__

# How do you add code in-line using markdown (a code span)?
*by wrapping content using a set of grave accents (backticks) `` ` ``*

__*`` `<h1>Encyclopedia Galactica</h1>` ``*__

# How do you add a single grave accent to a code span in markdown?
*by using double-graves with a one-space pad on either side. Pad is only needed in this special case of only one grave accent*

```markdown
`` ` ``

``just one ` grave accent.``

``a set of `grave` accents.``

```


# How do you add a pre-formatted code block using markdown?
*on the preceding line and following lines of the block, use triple grave accents (backticks) ` ``` `*

````
```
    Blazing wintertime
A deep, clever lake calls
    Darkening mountain
```
````

# How do you escape a triple-grave enclosed code-block surrounded by another markdown code-block?
*use an outer four-grave pair `` ```` `` and nest triple-graves accourdingly, if you need to escape a four-grave pair, use a five-grave pair. Use this pattern to escape markdown code-blocks ad infinitum*

```````
``````
`````
````
```
```
````
`````
``````
```````

# How do you add syntax highlighting to a pre-formatted code block in markdown?
*by adding a supported language just after the leading triple-grave of the code-block declaration.*

__*` ```html `*__

````
```html
<!DOCTYPE html>
<html>
<head>
    <title></title>
</head>
<body>
    <h1>The Mos Maiorum of the Roman Senate</h1>
</body>
</html>
```
````
__*GFM uses highlight.js to provide syntax highlighting.  [See the full list of supported languages](https://highlightjs.org/static/demo/)*__

# How do you add a table using github flavored markdown (GFM)?
*tables require headers. headers are created using a combination of pipe `|` and __at least__ three hypen symbols.`---`. Rows follow the same format and must be placed under the headers*

```markdown
  x   | column a  | column b | column c
---   |   --------|  ------- | ---
row 1 |  cell a1  |   cell b1| cell c1
row 2 |cell a2    | cell b2  |cell c2
row 3|cell a3|cell b3|cell c3
```
__*Note that the markdown you write does NOT need to be aligned*__

# How do you align the columns in a markdown (GFM) table?
*add a colon `:` to either side or both sides of the tables header dashes*

```markdown
:---    left align
:---:   center align
---:    right align
```

```markdown
  x   | left alignment| Center alignment  | Right alignment
---   |   :--------   |  :-------:       | ---:
row 1 |  *cell a1*    |   __*cell b1*__  | `cell c1`
row 2 |__cell a2__    | `cell b2`        |cell c2
row 3| *cell a3* |cell b3| _cell c3_
```
__*with the exception of headers `#`, Markdown styling may be applied to cell contents*__

# How do you add a blockquote using markdown?
*by preceding each line of the quoted text with the right-angle bracket `>` with a single padding space*

```markdown
> Here is important and/or quotable, attention should be drawn here.
```

```markdown
> Block
> quotes
> concatenate to a single line
> even
> with
> new
> lines.
```

# How do you add html directly to an markdown file?
*Since, relative to an html document, the use of markdown implies that we the html elements availble that can be children of the html `<body>` tag.  GFM when rendered on github may only have a subset of html elements available.*

```markdown
<dl>
    <dt>Supercalifragilisticexpialidocious</dt>
    <dd>Extraordinarily Good; Wonderful</dd>
</dl>
```

# How do you add a horizontal rule using markdown?
*use three or more hyphens, asterisks, or underscores. `---, ***, ___`*

```markdown
---
here is a section
***
here is another section
___
yet another section
```

# How do you add a youtube video using GFM markdown for use on Github?
*you can't, but you can use a linked image to send the viewer to youtube. `img.youtube.com` serves up video thumbnails*

`http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg`


```markdown
[![R2D2's Secret Message image]][R2D2's Secret Message video]

[R2D2's Secret Message image]: http://img.youtube.com/vi/Uj1ykZWtPYI/0.jpg
[R2D2's Secret Message video]: http://www.youtube.com/watch?v=Uj1ykZWtPYI
```
[![R2D2's Secret Message image]][R2D2's Secret Message video]

[R2D2's Secret Message image]: http://img.youtube.com/vi/Uj1ykZWtPYI/0.jpg
[R2D2's Secret Message video]: http://www.youtube.com/watch?v=Uj1ykZWtPYI