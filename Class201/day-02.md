# HTML Text
## Tags
Tags provide meaning and structure to the page of browsers



## Structural Tags
**Headings &lt;1 &gt;,&lt; 2 &gt;...:**    There are 6 levels to headings \
**Paragraph &lt;p&gt;:**    Creates a paragraph \
**Bold &lt;b&gt;:**    Bolds any charcter inside the opening and closing tags \
**Italic &lt;i&gt;:**    Italicizes any charcter inside the opening and closing tags \
**Superscript &lt;sup&gt;:**    Superscript charcters used in suffixes of dates or math concepts (2<sup>2</sup>)
**Subscript &lt;sub&gt;:**     Subscript characters used in footnotes or chem (H<sub>2</sub>0) \
**Line Breaks &lt;br /&gt;:**    Adds a line break into a paragraph \
**Horizontal Rules** &lt;hr /&gt;:**    Creates a line between ideas, like to change topic or a new scene in a play\

<hr />

## Semantic Tags - do not affect structure but adds extrea info to pages
**Strong &lt;strong&gt;:**    Indicates the element has strong importance \
**Emphasis &lt;&gt;:**    Indicatse emphasis \
**Blockquote &lt;blockquote&gt;:**    Long quotes that take up a whole paragraph \
**Quote &lt;q&gt;:**    Short quotes within a paragraph \
**Abbreviations&Acronyms &lt;abbr&gt;:**    Use a title attribute to specify full term \
**Citation &lt;cite&gt;:**    Used when referencing a piece of work (book, film, ect) \
**Definition &lt;dfn&gt;:**    Explaining new terminology /
**Author Details &lt;address&gt;:**    Contains contact info for author of the page \
**Insert &lt;ins&gt;:**    Used to show content was inserted into the document \
**Delete &lt;del&gt;:**    Used to show content was deleted from the document \
**Strike-out &lt;s&gt;:**    Used to show content is not longer accurate/relevant but should not be deleted 



# CSS Intro

## CSS works with HTML elements to tell the page how they should be displayed
* Contains 2 parts
  * Selector/element (h1, p, body)
  * Declaration (how it will be styled) - done in two parts
    * property: name of the style (color, font, size)
    * value: specify the color, size, ect

Examples: \
h1 { \
  font-family: Arial; \
  color: blue; \
} 

## External & Internal CSS
* External is linked using:
&lt;link href="css/styles.css" type="text/css" rel="stylesheet"&gt;
  * Requires less code in html and allows all pages to share the same stylesheet
* Internal uses the html tag &lt;style&gt;
  * Everything is in one file

## Selectors there are many kinds, some most common ones:

**Universal Selector** * {}:    Applies to all elements \
**Type Selector** h1, h2, h3 {}:    Matches element name \
**Class Selector** .className {}:    Matches to class attribute \
**ID Selector** #IDName {}: Matches to an ID attribute \
**Child Selector** li&lt;a {}: Matches an element that is a direct child of another \



## Basic Javascript Instructions

| Term | How it's applied | Definition|
|------|------------------|-----------|
| Statement | Ends with ; | An individual step/instruction |
| Comment | Single line comment: // Multi-line: /* jkdfalj */ | Comments are used to explain code |
| Variables | var variableName | Store information from a statement |
| Array | Declare variable then name the array [] | A list of values |
| Expressions | var area = 3*2 | turns a single value or multiple values into a single value |
| Operators | + = * | Create a single value from 1+ |

## Decisions and Loops

### Comparison Operators
* Return a boolean

| Operator | Definition | Example |
|----------|------------|---------|
| == | equal to | 4 == 5 : false |
| != | not equal to | 4 != 5 : true |
| === | strict equal to | 'one' === 1 : false |
| !== | strict not equal to | 'one' !== 1 : true |
|  &gt; | greater than | 8 > 4 : true |
| &lt; | less than | 8 < 4 : false |
| &gt;= | greater than or equal to | 8 &gt;= 8 : true |
| &lt;= | less than or equal to | 8 &lt;= 8 : true |

### Logical Operators

* Allows you to compare multiple comparison operators
* && logical and
* || logical or
* ! logical not

### If Statements

* Evaluate a condition to see if true

if (score >= 50) {                <-- If variable score is greater than 50 \
 congratulate();                      run congratulate function \
}     \
