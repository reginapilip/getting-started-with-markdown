# Markdown Syntax

This is an introduction to the *basic* Markdown syntax. Markdown has an *extended syntax*. 

If you want to learn more, visit the **Markdown Resources** lesson in this repository.

**QUICK REFERENCE**
- [Markdown Syntax](#markdown-syntax)
  - [Headings](#headings)
  - [Paragraphs](#paragraphs)
  - [Emphasis](#emphasis)
  - [Blockquotes](#blockquotes)
    - [Regular Blockquote](#regular-blockquote)
    - [Blockquotes with Multiple Paragraphs](#blockquotes-with-multiple-paragraphs)
    - [Nested Blockquotes](#nested-blockquotes)
    - [Blockquotes with Elements](#blockquotes-with-elements)
  - [Lists](#lists)
    - [Ordered Lists](#ordered-lists)
    - [Unordered Lists](#unordered-lists)
    - [Nesting Lists](#nesting-lists)
    - [Incorporating Elements within Lists](#incorporating-elements-within-lists)
  - [Code](#code)
    - [Inline Code](#inline-code)
    - [Fenced Code Blocks](#fenced-code-blocks)
  - [Links](#links)
  - [Images](#images)
  - [Escaping Characters](#escaping-characters)
  - [HTML](#html)
  - [Tables](#tables)

## Headings

```markdown
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```

**Best Practices**

Make sure to leave a space between the pound sign and the heading text

## Paragraphs

```markdown
No special characters needed - just start typing!

This is the start of a paragraph.

Here's another paragraph. Notice that I just start on a new line to start a new paragraph. Markdown honors the line breaks.
```

**Best Practices**
- Don't indent or put tabs or spaces to format the beginning of your paragraphs. 

```markdown
Example:
  Don't do this - notice the indent at the start of this new line?
```

## Emphasis

Note: depending on what editor you are using, underscores may not work. Best practice is to use asterisks.

```markdown
<!-- BOLD -->
**This text is bold** - two asterisks
__This text is also bold__ - two underscores

<!-- ITALICS -->
*This text is italicized* - one asterisk
_This text is also italicized_ - one underscore

<!-- BOLD + ITALICS -->
***This text is bold and italicized*** - three asterisks
___This text is also bold and italicized___ - three underscores 
__*This sentence too*__ - 2 underscore + 1 asterisk
**_And this one_** - 2 asterisks + 1 underscore
```

## Blockquotes

Add a `>` in front of a paragraph

### Regular Blockquote
```markdown
> This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. 
```
**Preview:**
> This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. 

### Blockquotes with Multiple Paragraphs

```markdown
> This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote.
>
> This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote.
```
**Preview:**
> This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote.
>
> This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote. This is 

### Nested Blockquotes
```markdown
> This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote.
>> This is my nested blockquote. This is my nested blockquote. This is my nested blockquote.
```
**Preview:**
> This is my blockquote. This is my blockquote. This is my blockquote. This is my blockquote.
>> This is my nested blockquote. This is my nested blockquote. This is my nested blockquote.

### Blockquotes with Elements

You can use other Markdown elements within blockquotes - you just need to experiment to see which ones you can use.

Here's an example:
```markdown
> ## Blockquote Header
> - List item 1
> - List item 2
> This tests *italics* and **bold**.
```
**Preview:**
> ## Blockquote Header
> - List item 1
> - List item 2
> This tests *italics* and **bold**.

## Lists

There are two types of lists: **Ordered Lists** and **Unordered Lists**

**Ordered Lists** look like this:
1. List item 
2. List item

**Unordered Lists** look like this:
- List item
- List item

### Ordered Lists
```markdown
1. First item
2. Second item
3. Third item
4. Fourth item
```

### Unordered Lists
```markdown
- First item
- Second item
- Third item
- Fourth item

<!-- Alternative syntax: -->
* First item
* Second item

+ First item
+ Second item

+ First item
- Second item
* Third item
```

### Nesting Lists
```markdown
<!-- use tab -->
- List item 1
  - Nested list item 
    - Nested list item
```

### Incorporating Elements within Lists

```markdown
- List item 1 
- List item 2

  I want to add a paragraph right here, under List item 2. Make sure to tab this paragraph once or use 4 spaces

  > I also want to add a blockquote.

- List item 3 
- List item 4
- List item 5
```
**Preview:**

- List item 1 
- List item 2

  I want to add a paragraph right here, under List item 2. Make sure to tab this paragraph once or use 4 spaces

  > I also want to add a blockquote.

- List item 3 
- List item 4
- List item 5



## Code

### Inline Code
```markdown
<!-- use single back ticks -->
Type in `<h1>Hello World!</h1>` within the body tag of your HTML file.
```

### Fenced Code Blocks

Depending on your Markdown processor, you will use 3 backticks (```) or 3 tildes (~~~) to create a code block.

Example: 
\```

{

  "firstName": "Regina",

  "lastName": "Pilipchuk"

}

\```


\```json

{

  "firstName": "Regina",

  "lastName": "Pilipchuk"

}

\```


## Links

```markdown
[Link description](URL "title") - title is optional

<!-- example -->
[Markdown Guide](https://www.markdownguide.org/basic-syntax/ "Markdown Basic Syntax Guide")
```
**Preview of Example:**

[Markdown Guide](https://www.markdownguide.org/basic-syntax/ "Markdown Basic Syntax Guide")

## Images

```markdown
![Alt text](absolute/relative path to image)

<!-- example -->
![Picture of a cat](https://picsum.photos/id/237/200/300)
```
**Preview of Example:**

![Picture of a cat](https://picsum.photos/id/237/200/300)


## Escaping Characters

Characters you can escape:
| Character | Name              |
| --------- | ----------------- |
| \         | backslash         |
| `         | backtick          |
| *         | asterisk          |
| _         | underscore        |
| {}        | curly braces      |
| []        | brackets          |
| ()        | parantheses       |
| #         | pound sign        |
| +         | plus sign         |
| -         | minus sign/hyphen |
| .         | dot/period        |
| \|        | pipe              |

```markdown
<!-- use a backslash \ -->
The phrase "not code" won't render as code because the backticks are escaped: \`not code\`
```

Using backslashes: \`not code\`

Not using backslashes: `not code`

## HTML

You can use HTML tags within your Markdown too. Here are some examples:

```markdown
<!-- example code -->
This <strong>word</strong> is bold. This one is <em>italicized</em>.

<img src="https://www.humanesociety.org/sites/default/files/styles/1240x698/public/2018/08/kitten-440379.jpg?h=c8d00152&itok=1fdekAh2" alt="Picture of a cat using HTML image tag">
```
**Preview:**

This <strong>word</strong> is bold. This one is <em>italicized</em>.

<img src="https://www.humanesociety.org/sites/default/files/styles/1240x698/public/2018/08/kitten-440379.jpg?h=c8d00152&itok=1fdekAh2" alt="Picture of a cat using HTML image tag">

## Tables

```markdown
| Name   | Color |
| ------ | ----- |
| Regina | blue  |
```
**Preview**

| Name   | Color |
| ------ | ----- |
| Regina | blue  |