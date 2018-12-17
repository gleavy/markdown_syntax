# Markdown Syntax
A list of GitHub-flavoured Markdown with examples.

Markdown is a light markup language often used for READMEs.
There are many different dialects/flavours of Markdown - all are pretty much the same, with only minor differences - but this document 
will focus on GitHub-flavoured Markdown.

---

# Summary

| Style                                                                                                                  | Syntax                         | Example             | Output            |
| ---------------------------------------------------------------------------------------------------------------------- | ------------------------------ | ------------------- | ----------------- |
| [Headings](https://github.com/gleavy/markdown_syntax/new/master?readme=1#headings)                                     | `# `                           | `#### Header 4`     |                   |
| [Horizontal Rule](https://github.com/gleavy/markdown_syntax/new/master?readme=1#horizontal-rule)                       | `---`, `***`, `___`            | `---`               |                   |
| [Bold](https://github.com/gleavy/markdown_syntax/new/master?readme=1#bold)                                             | `** **`                        | `**Bold**`          | **Bold**          |
| [Italic](https://github.com/gleavy/markdown_syntax/new/master?readme=1#italic)                                         | `* *` or `_ _`                 | `*Italic*`          | *Italic*          |
| [Strikethrough](https://github.com/gleavy/markdown_syntax/new/master?readme=1#strikethrough)                           | `~~ ~~`                        | `~~Strikethrough~~` | ~~Strikethrough~~ |
| [Quoting Text](https://github.com/gleavy/markdown_syntax/new/master?readme=1#quoting-text)                             | `> `                           | `> I am Groot`      |                   |
| [Quoting Code](https://github.com/gleavy/markdown_syntax/new/master?readme=1#quoting-code)                             | ``` ` ```                      |                     | `Code`            |
| [Lists](https://github.com/gleavy/markdown_syntax/new/master?readme=1#lists)                                           | `-`, `*`, `1`, ` [ ]`, ` [x]`  | `- Python`          |                   |  
| [Tables](https://github.com/gleavy/markdown_syntax/new/master?readme=1#tables)                                         | `|`, `-`                       |                     |                   | 
| [Links](https://github.com/gleavy/markdown_syntax/new/master?readme=1#links)                                           | `[]()`                         | `[Google](www.google.com)` | [Google](www.google.com) |
| [Paragraphs & Line Breaks](https://github.com/gleavy/markdown_syntax/new/master?readme=1#paragraphs-and-line-breaks-1) |
| [Ignoring Markdown Format](https://github.com/gleavy/markdown_syntax/new/master?readme=1#ignore-markdown-formatting)   | `\`                            | `\*new-file-name\*` | \*new-file-name\* |   
| [Mentioning People & Teams](https://github.com/gleavy/markdown_syntax/new/master?readme=1#mentioning-people--teams)    | `@`                            | `@organization/team` |                  |
| [Referencing Issues & Pull Requests](https://github.com/gleavy/markdown_syntax/new/master?readme=1#referencing-issues--pull-requests)                   | `#`                 |                   |
| [Content Attachments](https://github.com/gleavy/markdown_syntax/new/master?readme=1#content-attachments)               |                                | |
| [Using Emoji](https://github.com/gleavy/markdown_syntax/new/master?readme=1#using-emoji)                               | `: :`                          | `:+1:`              | :+1:              |

---

# Headings
Prefix with # and a space `# `. The number of #s (up to 6) defines the depth of the heading tag.
```
# h1 - The largest heading - an \<h1\> tag
## h2 - The second largest heading
### h3
#### h4
##### h5
###### h6 - The smallest heading
```

# h1 - The largest heading - an \<h1\> tag
## h2 - The second largest heading
### h3
#### h4
##### h5
###### h6 - The smallest heading

---

# Horizontal Rule
Use three or more `---`, `***`, or `___`.
`---`

---

# Styling Text

## Bold
Surround with double asterisks `**`.

`This is a **bold** example.`

This is a **bold** example.


## Italics
Surround with single underscores `_` or single asterisks `*`.

`This is an _italics_ example, and so is *this*.`

This is an _italics_ example, and so is *this*.


## Bold & Italics

`This example is in **bold and includes _italics_.**`

This example is in **bold and includes _italics_.**


## Strikethrough
Surround with double tildes `~~`.

`Strikethrough the next three words: ~~strike out these~~, but not anything after them.`

Strikethrough the next three words: ~~strike out these~~, but not anything after them.

---

# Quoting Text
Prefix with `> `.

```
In the words of Abraham Lincoln:
> Four score and seven years ago ...
```

In the words of Abraham Lincoln:
> Four score and seven years ago ...


# Quoting Code
Call out code or a command in a sentence with `single backticks` ``` ` ```. The text within the backticks will not be formatted.
Use `git status` to list all new or modified files that haven't yet been committed.

To format code or text into its own distinct block, use `triple backticks` .
Some basic Git commands are:
```
git status
git add
git commit
```

# Quoting Code with Syntax Highlighting
Within code blocks, you can add an optional language identifier to enable syntax highlighting in the fenced code block.

```
```python
def square_number(x):
    return x * x
\``` 
```

```python
def square_number(x):
    return x * x
```

---

# Lists
## Unordered Lists
Precede each line with a `-`, `+`, or `*`
```
- Groucho Marx
- Chico Marx
- Harpo Marx
```

- Groucho Marx
- Chico Marx
- Harpo Marx


## Ordered Lists
Precede each line with a number `1.`
```
1. Curly
2. Larry
3. Moe
```

1. Curly
2. Larry
3. Moe

## Task Lists
Preface list items with a regular space character follow by square brackets ` [ ]`. To mark a task as complete, use `[x]`
```
- [x] Finish my changes
- [ ] Push my commits to GitHub
- [ ] Open a pull request
```

- [x] Finish my changes
- [ ] Push my commits to GitHub
- [ ] Open a pull request

## Nest Lists
Create a nested list by indenting, and use spaces to align.
```
1. First list item
   - First nested list item
     - Second nested list item
2. Second list item
```

1. First list item
   - First nested list item
     - Second nested list item
2. Second list item

    
---

# Tables
**Note:** Tables are now part of the core Mardown spec, and rendering will depend on the tool being used.

Tables are created using pipes `|` and hypens `-`. 
- Hypens are used to create each column's header - there must be at least 3 hypens in each column of the header row.
- Pipes separate each column (but are pptional at either end of the table).
- You must include a blank line before a table in order for it to render correctly.
- Cells can vary in width and do not need to be perfectly aligned.

```
| First Header | Second Header |
| ------------ | ------------- |
| Content Cell | Content Cell  |
| Content Cell | Content Cell  |
``` 

| First Header | Second Header |
| ------------ | ------------- |
| Content Cell | Content Cell  |
| Content Cell | Content Cell  |


Text can be aligned within a column by using colons in the header row. The tool used will determine if this is 
```
| Left-aligned | Center-aligned | Right-aligned |
| :---         | :---:          |          ---: |
| left         | center         | right         |
| left         | center         | right         |
``` 

| Left-aligned | Center-aligned | Right-aligned |
| :----------- | -------------- | ------------- |
| left         | center         | right         |
| left         | center         | right         |

---

# Links
Wrap the link text in square brackets `[]`, immediately followed by the URL wrapped in parentheses `()`.
For example, 
`This site was built using [GitHub Pages](https://pages.github.com)`.

This site was building using [GitHub Pages](https://pages.github.com)


## Section Links
You can link directly to a section in a rendered Markdown file by hovering over the heading to expose the link. 
Use that link to create a regular link, as above.


## Relative Links
You can define relative links and image paths in your rendered Markdown files to help readers to navigate to other files 
in your repository. GitHub recommends using relative links instead of absolute links (these may not work in clones of your repository).
You can use relative link operands such as `./` and `../`.

A relative link  is a link that is relative to the current file. For example, if you have a README file in the root of your 
repository, and you have another file in *docs/CONTRIBUTING.md*, the relative link to *CONTRIBUTING.md* in your README might look like
`[Contribution guidelines for this project](docs/CONTRIBUTING.md)`

---

# Paragraphs and Line Breaks
These can be challenging; experiment with multiple newlines.

---

# Ignore Markdown Formatting
Use `\` before the Markdown character. Markdown provides backslash escapes for the following characters:

|               |                      |                      |
| ------------- | -------------------- | -------------------- | 
| \\  backslash | \+ plus sign         |  \(\) parantheses    | 
| \` backtick   | \- minus sign        | \{\} curly braces    |
| \* asterisk   | \. dot               | \[\] square brackets |
| \_ underscore | \! exclaimation mark | \#  hashmark         |




`Let's rename \*our-new-project\* to \*our-old-project\*.` 

Let's rename \*our-new-project\* to \*our-old-project\*.

---

# Mentioning People & Teams
Mention a person or team using `@`. This triggers a notification.
`@organization/team When is the next commit?`

---

# Referencing Issues & Pull Requests
Using `#`, you can filter the list of issues and requests.

`#`

`GH-`

`Username/Repository#`

`Organization_name/Repository#`


---

# Content Attachments
Some GitHub apps provide information in GitHub for URLs that link to their registered domains. GitHub renders the information 
provided by the app under the URL in the body or comment of an issue or pull request.

To see the content attachments, you must have a GitHub app that uses the Content Attachments API installed on the repository.

---

# Using Emoji
Surround  emoji code with colons `:`. A complete list of supported emoji images is avaiable at [http://www.emoji-cheat-sheet.com](www.emoji-cheat-sheet.com)
`:+1: :shipit:`

:+1: :shipit:
