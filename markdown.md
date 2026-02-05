<!--This means we can use HTML elements in Markdown, such as the comment
element, and they won't be affected by a markdown parser. However, if you
create an HTML element in your markdown file, you cannot use markdown syntax
within that element's contents.-->
# This is an <h1>
## This is an <h2>
### This is an <h3>
#### This is an <h4>
##### This is an <h5>
###### This is an <h6>
This is an h1
=============

This is an h2
-------------
*This text is in italics.*
_And so is this text._

**This text is in bold.**
__And so is this text.__

***This text is in both.***
**_As is this!_**
*__And this!__*
~~This text is rendered with strikethrough.~~
This is a paragraph. I'm typing in a paragraph isn't this fun?

Now I'm in paragraph 2.
I'm still in paragraph 2 too!


I'm in paragraph three!
I end with two spaces (highlight me to see them).

There's a <br /> above me!
> This is a block quote. You can either
> manually wrap your lines and put a `>` before every line or you can let your lines get really long and wrap on their own.
> It doesn't make a difference so long as they start with a `>`.

> You can also use more than one level
>> of indentation?
> How neat is that?

* Item
* Item
* Another item

or

+ Item
+ Item
+ One more item

or

- Item
- Item
- One last item
1. Item one
2. Item two
3. Item three
1. Item one
1. Item two
1. Item three
1. Item one
2. Item two
3. Item three
    * Sub-item
    * Sub-item
4. Item four
Boxes below without the 'x' are unchecked HTML checkboxes.
- [ ] First task to complete.
- [ ] Second task that needs done
This checkbox below will be a checked HTML checkbox.
- [x] This task has been completed
    This is code
    So is this
    my_array.each do |item|
      puts item
    end
John didn't even know what the `go_to()` function did!
***
---
- - -
****************
[Click me!](http://test.com/)
[Click me!](http://test.com/ "Link to Test.com")
[Go to music](/music/).
[Click this link][link1] for more info about it!
[Also check out this link][foobar] if you want to.

[link1]: http://test.com/ "Cool!"
[foobar]: http://foobar.biz/ "Alright!"
[This][] is a link.

[This]: http://thisisalink.com/
- [Heading](#heading)
- [Another heading](#another-heading)
- [Chapter](#chapter)
  - [Subchapter <h3 />](#subchapter-h3-)
![This is the alt-attribute for my image](http://imgur.com/myimage.jpg "An optional title")
![This is the alt-attribute.][myimage]

[myimage]: relative/urls/cool/image.jpg "if you need a title, it's here"
<http://testwebsite.com/> is equivalent to
[http://testwebsite.com/](http://testwebsite.com/)
<foo@bar.com>
I want to type *this text surrounded by asterisks* but I don't want it to be
in italics, so I do this: \*this text surrounded by asterisks\*.
Your computer crashed? Try sending a
<kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd>
| Col1         | Col2     | Col3          |
| :----------- | :------: | ------------: |
| Left-aligned | Centered | Right-aligned |
| blah         | blah     | blah          |
Col 1 | Col2 | Col3
:-- | :-: | --:
Ugh this is so ugly | make it | stop

## Backslash Escapes
https://daringfireball.net/projects/markdown/syntax#precode

**syntax**
```
\*literal asterisks\*
```
**output**

\*literal asterisks\*
****************************
## More than one new Line
**syntax**
```
\
\
\
Two blank lines above
<br/><br/><br/>
Two blank lines above
```
**output**
\
\
\
Two blank lines above
<br/><br/><br/>
Two blank lines above
****************************
## Emoji
http://www.emoji-cheat-sheet.com/
https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md

**syntax**
```
:+1: :sparkles: :camel: :tada:
:rocket: :metal: :octocat:
GitHub supports emoji!
```
**output**
:+1: :sparkles: :camel: :tada:
:rocket: :metal: :octocat:
GitHub supports emoji!
****************************
## How can I reference a commit, issue, PR etc in an issue comment on GitHub?
[Autolinked references and URLs](https://docs.github.com/en/github/writing-on-github/working-with-advanced-formatting/autolinked-references-and-urls)
****************************
## Username @mentions
Mention person or team

https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#mentioning-people-and-teams
****************************
## Tables
To create a table with headers we need to use dashes to separate each header cell and use pipes to separate columns. The outer pipes are optional. We can use any number of dashes and spaces to increase readability. We can use colons to align columns. For left-align text, use a colon to the left of dashes. For center-align text, use a colon on both sides of dashes. For right-align text, use a colon to the right of dashes. By default Left align is used.

**syntax**
```
First Header | Second Header
-|-
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

<table>
  <tr>
    <th>First Header</th>
    <th>Second Header</th>
  </tr>
  <tr>
    <td>Content from cell 1</td>
    <td>Content from cell 2</td>
  </tr>
  <tr>
    <td>Content in the first column</td>
    <td>Content in the second column</td>
  </tr>
</table>

Default | Left align | Center align | Right align
-- | :- | :-: | -: |
9999999999 | 9999999999 | 9999999999 | 9999999999
999999999 | 999999999 | 999999999 | 999999999
99999999 | 99999999 | 99999999 | 99999999
9999999 | 9999999 | 9999999 | 9999999

Now display two tables side by side.

<table>
<tr>
<th>Heading 1</th>
<th>Heading 2</th>
</tr>
<tr>

<td>

| A | B | C |
|--|--|--|
| 1 | 2 | 3 |

</td><td>

| A | B | C |
|--|--|--|
| 1 | 2 | 3 |

</td></tr> </table>

Let’s create a table with multiple lines using the HTML <br/> tag.

| A | B | C |
|---|---|---|
| 1 | 2 | 3 <br/> 4 <br/> 5 |

```
**output**
First Header | Second Header
-|-
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

<table>
  <tr>
    <th>First Header</th>
    <th>Second Header</th>
  </tr>
  <tr>
    <td>Content from cell 1</td>
    <td>Content from cell 2</td>
  </tr>
  <tr>
    <td>Content in the first column</td>
    <td>Content in the second column</td>
  </tr>
</table>

Default | Left align | Center align | Right align
-- | :- | :-: | -: |
9999999999 | 9999999999 | 9999999999 | 9999999999
999999999 | 999999999 | 999999999 | 999999999
99999999 | 99999999 | 99999999 | 99999999
9999999 | 9999999 | 9999999 | 9999999

Now display two tables side by side.

<table>
<tr>
<th>Heading 1</th>
<th>Heading 2</th>
</tr>
<tr>

<td>

| A | B | C |
|--|--|--|
| 1 | 2 | 3 |

</td><td>

| A | B | C |
|--|--|--|
| 1 | 2 | 3 |

</td></tr> </table>

Let’s create a table with multiple lines using the HTML <br/> tag.

| A | B | C |
|---|---|---|
| 1 | 2 | 3 <br/> 4 <br/> 5 |

****************************
## Task lists
**syntax**
```
- [x] Finish my changes
- [ ] Push my commits to GitHub
- [ ] Open a pull request

If a task list item description begins with a parenthesis, you'll need to escape it with \:

- [ ] \(Optional) Open a followup issue
```
**output**
- [x] Finish my changes
- [ ] Push my commits to GitHub
- [ ] Open a pull request

- [ ] \(Optional) Open a followup issue
****************************
## Lists
**syntax**
```
You can make an unordered list by preceding one or more lines of text with - or *.

- George Washington
- John Adams
- Thomas Jefferson

To order your list, precede each line with a number.

1. James Madison
2. James Monroe
3. John Quincy Adams
```
**output**

You can make an unordered list by preceding one or more lines of text with - or *.

- George Washington
- John Adams
- Thomas Jefferson

To order your list, precede each line with a number.

1. James Madison
2. James Monroe
3. John Quincy Adams
****************************
## Nested Lists
You can create a nested list by indenting one or more list items below another item.

To create a nested list using the web editor on GitHub or a text editor that uses a monospaced font, like Atom, you can align your list visually. Type space characters in front of your nested list item, until the list marker character (- or *) lies directly below the first character of the text in the item above it.
**syntax**
```
In this example, you could add a nested list item under the list item 100. First list item by indenting the nested list item a minimum of five spaces, since there are five characters (100. ) before First list item.

100. First list item
     - First nested list item

You can create multiple levels of nested lists using the same method. For example, because the first nested list item has seven spaces (␣␣␣␣␣-␣) before the nested list content First nested list item, you would need to indent the second nested list item by seven spaces.

100. First list item
     - First nested list item
       - Second nested list item
```
**output**

100. First list item
     - First nested list item
       - Second nested list item
****************************
## Horizontal rules
**syntax**
```
***
---
<hr/>
```
**output**
***
****************************
## Links & images
**syntax**
```
[GitHub Pages](https://pages.github.com/)
[GitHub Pages](https://pages.github.com/ "With a Title")
![image](https://nikhilnayyar.web.app/_assets/img/avatar.jpg)
[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)
[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)
```
**output**
[GitHub Pages](https://pages.github.com/)
[GitHub Pages](https://pages.github.com/ "With a Title")
![image](https://nikhilnayyar.web.app/_assets/img/avatar.jpg)
[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)
[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)
****************************
## Reference-style links
If you’re using the same link more the once, then using the reference style would be beneficial since you don’t have to write the link every time, and also, it’s easy to update the link. Moreover, you can use numbers for the reference text. Also, you can use the reference text as the link text.

https://daringfireball.net/projects/markdown/syntax#link
https://daringfireball.net/projects/markdown/syntax#img

**syntax**
```
[The-Ultimate-Markdown-Cheat-Sheet][reference text]
[The-Ultimate-Markdown-Cheat-Sheet][1]
[Markdown-Cheat-Sheet]
![Alt text][image-1]

[reference text]: https://github.com/lifeparticle/The-Ultimate-Markdown-Cheat-Sheet
[1]: https://github.com/lifeparticle/The-Ultimate-Markdown-Cheat-Sheet
[Markdown-Cheat-Sheet]: https://github.com/lifeparticle/The-Ultimate-Markdown-Cheat-Sheet
[image-1]: https://media.giphy.com/media/qLHzYjlA2FW8g/giphy.gif
```
**output**

[The-Ultimate-Markdown-Cheat-Sheet][reference text]
[The-Ultimate-Markdown-Cheat-Sheet][1]
[Markdown-Cheat-Sheet]
![Alt text][image-1]

[reference text]: https://github.com/lifeparticle/The-Ultimate-Markdown-Cheat-Sheet
[1]: https://github.com/lifeparticle/The-Ultimate-Markdown-Cheat-Sheet "With a Title"
[Markdown-Cheat-Sheet]: https://github.com/lifeparticle/The-Ultimate-Markdown-Cheat-Sheet
[image-1]: https://media.giphy.com/media/qLHzYjlA2FW8g/giphy.gif
****************************
## Section links
You can link directly to a section in a rendered file by hovering over the section heading to expose the link:

![image](https://docs.github.com/assets/images/help/repository/readme-links.png)

Also read this stackoverflow comment for manually creating links [how-to-link-to-part-of-the-same-document-in-markdown](https://stackoverflow.com/a/72756103)
****************************
## Relative links
A relative link is a link that is relative to the current file. For example, if you have a README file in root of your repository, and you have another file in docs/CONTRIBUTING.md, the relative link to CONTRIBUTING.md in your README might look like this:
```
[Contribution guidelines for this project](docs/CONTRIBUTING.md)
```
GitHub will automatically transform your relative link or image path based on whatever branch you're currently on, so that the link or path always works. You can use all relative link operands, such as ./ and ../.
****************************
## Quoting code
**syntax**
<pre>
Use `git status` to list all new or modified files that haven't yet been committed.

To format code or text into its own distinct block, use triple backticks.
```
git status
git add
git commit
```
```c++
#include<iostream>
using namespace std;
```
```diff
  Unchanged Line
- Removed Line
+ Added Line
```
```scss
.header {
 color: red;
}
</pre>
**output**
Use `git status` to list all new or modified files that haven't yet been committed.

To format code or text into its own distinct block, use triple backticks.
```
git status
git add
git commit
```
```c++
#include<iostream>
using namespace std;
```
```diff
  Unchanged Line
- Removed Line
+ Added Line
```
```scss
.header {
 color: red;
}
```
****************************
## Headers
**syntax**
```
# H1
## H2
### H3
#### H4
##### H5
###### H6
```
**output**
# H1
## H2
### H3
#### H4
##### H5
###### H6
****************************
## Text
**syntax**
```
**Bold**
*Italic*
***Bold-Italic***
<del>deleted</del>
~~This was mistaken text~~
<ins>inserted</ins>
a<sub>subscripted</sub>
a<sup>superscripted</sup>
<samp>Monospaced</samp>
<table><tr><td>Boxed</td></tr></table>
<kbd>button</kbd>
<code>highlight</code>

`highlight`
```
**output**

**Bold**
*Italic*
***Bold-Italic***
<del>deleted</del>
~~This was mistaken text~~
<ins>inserted</ins>
a<sub>subscripted</sub>
a<sup>superscripted</sup>
<samp>Monospaced</samp>
<table><tr><td>Boxed</td></tr></table>
<kbd>button</kbd>
<code>highlight</code>

`highlight`

****************************
## Block Quotes
**syntax**
```
> The quick brown fox jumps over the lazy dog.
> The quick brown fox jumps over the lazy dog.

> The quick brown fox jumps over the lazy dog.
> 

> The quick brown fox jumps over the lazy dog.
> The quick brown fox jumps over the lazy dog.
>> The quick brown fox jumps over the lazy dog.
>>> The quick brown fox jumps over the lazy dog.

> **The quick brown fox** *jumps over the lazy dog.*

<blockquote>
hi there<br/>
is a good way
</blockquote>
```
**output**

> The quick brown fox jumps over the lazy dog.
> The quick brown fox jumps over the lazy dog.

> The quick brown fox jumps over the lazy dog.
> 

> The quick brown fox jumps over the lazy dog.
> The quick brown fox jumps over the lazy dog.
>> The quick brown fox jumps over the lazy dog.
>>> The quick brown fox jumps over the lazy dog.

> **The quick brown fox** *jumps over the lazy dog.*

<blockquote>
hi there<br/>
is a good way
</blockquote>

****************************
## Allignments
`<p align="center">` is used for alignment. Also note that images have border: `<img .. border="10"`.

**syntax**
```
<p align="center">
<img src="https://images.unsplash.com/photo-1415604934674-561df9abf539?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2772&q=80" width="100" height="100" border="10"/>
</p>
<p align="right">
<img src="https://images.unsplash.com/photo-1415604934674-561df9abf539?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2772&q=80" width="100" height="100" border="10"/>
</p>

```
**output**

<p align="center">
<img src="https://images.unsplash.com/photo-1415604934674-561df9abf539?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2772&q=80" width="100" height="100" border="10"/>
</p>
<p align="right">
<img src="https://images.unsplash.com/photo-1415604934674-561df9abf539?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2772&q=80" width="100" height="100" border="10"/>
</p>

****************************
## Comments
**syntax**
```
<!--
Lorem ipsum dolor sit amet
-->
```
****************************
## `<details>` html tag
**syntax**
```
<details>
    <summary>Details</summary>
    Something small enough to escape casual notice.
</details>
```
**output**
<details>
    <summary>Details</summary>
    Something small enough to escape casual notice.
</details>

****************************
## Bookmarks ( jump to specific parts of a page)
**syntax**
```
See [Optional Features](#optional-features)
#### Optional Features
```
**output**

See [Optional Features](#optional-features)
#### Optional Features
****************************
## Visualise Hex color code
works in comments, issue, prs.

**syntax**
```
`#00BFFF`
```
**output**

`#00BFFF`

**img output**

![image](https://user-images.githubusercontent.com/38173563/179364604-b378d9d8-c361-4035-a426-91d31cea6058.png)
****************************
