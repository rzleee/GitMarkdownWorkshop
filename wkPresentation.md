# Installation 
Visual Studio Code : https://code.visualstudio.com/

Pandoc             : https://pandoc.org/installing.html

Git installation   : https://git-scm.com/download/win

---
### Latex

 Windows : https://miktex.org/download
 
 OSX : http://www.tug.org/mactex/
 
 Linux : https://www.tug.org/texlive/

---
### GitHub
Creating a github account: https://github.com/

For pro account, you can link school email address to get benefits: https://education.github.com/discount_requests/new


# What is markdown
Markdown is a text-to-HTML conversion tool for web writers. 

Markdown allows you to write using an easy-to-read, easy-to-write plain text format, then convert it to structurally valid XHTML (or HTML).

Markdown is now commonly used to write README for Github.

# History
John Gruber created markdown after being frustated with writing long html tags to format his content.

So he created markdown which makes web based document easier to read and write.

# Example 
To look like this : The *quick* brown fox, jumped **over** the lazy [dog](https://en.wikipedia.org/wiki/Dog). 

Html:
```
The <i>quick</i> brown fox, jump <strong>over the lazy</strong> <a href="https://en.wikipedia.org/wiki/Dog"> dog </a>
```
Markdown: 
```
The *quick* brown fox, jumped **over** the lazy [dog](https://en.wikipedia.org/wiki/Dog).
```

# Why writers love markdown so much ?
 You have to pause your writing once awhile to reach over the mouse in order to click a formatting button, then click back to where you left off to continue.

Markdown allows us to keep our fingers on keyboard as we write any documents. It might seem like a small detail but it has a big effect. Once you start writing, it's hard to go back.

While novice users will find buttons a bit easier to use, advanced writers often swear by markdown and nothing else due to ***writing flow***. 

# Basic Markdown
Code Block

> **C**

\`\`\`C

int main(void){

   printf("Hello world");

}
\`\`\`


```C
int main(void){
    printf("Hello world");
}
```

> **Python**

\`\`\`python

s = "Python syntax highlighting"

print s

\`\`\`
```python
s = "Python syntax highlighting"
print s
```
```

```python
s = "Python syntax highlighting"
print s
```
# Headings
``` 
Headers
# Heading 1
## Heading 2
### Heading 3
```
# Heading 1
## Heading 2
### Heading 3
# Text
```
Text
*italic*
**bold**
***bold-italic***
```

*italic*

**bold**

***bold-italic***


# Link
```
[link](https://example.com)

```
[link](https://example.com)

# Image
```
Image
![m'lady](https://i.imgur.com/v8IVDka.jpg)
```
![m'lady](https://i.imgur.com/v8IVDka.jpg)

# List
```
List
* Unordered 1
	* Subunordered 1

1. Ordered 1
2. Ordered 2
3. Ordered 3
```
* Unordered 1
	* Subunordered 2

1. Ordered 1
2. Ordered 2
3. Ordered 3

# Quote
```
> Quote
```
> Quote

# Table
```
Horizontal Rules
---- 
```
---
```
Table
 Tables        | Are           | Cool  
 ------------- |:-------------:| -----:
 col 3 is      | right-aligned | $1600 
 col 2 is      | centered      |   $12 
 zebra stripes | are neat      |    $1 
 [Introduction](#&nbsp;Installation ) |  jumping     |    spaces 
 [Hyperlink](testing.txt) | redirect      |    files 

```
 
Tables        | Are           | Cool  
------------- |:-------------:| -----:
col 3 is      | right-aligned | $1600 
col 2 is      | centered      |   $12 
[Introduction](#&nbsp;Installation ) |  jumping     |    spaces 
[Hyperlink](testing.txt) | redirect      |    files 

# Escape
```
Escape
\*literally\* 

```
\*literally\* 

# File conversion with Pandoc

# Introduction to pandoc 
If you need to convert files from one markup format into another, pandoc is your swiss-army knife.

Pandoc is a Haskell library for converting from one markup format to another, and a command-line tool that uses this library.



# Conversion

Convert Markdown to HTML : pandoc -f markdown -t html5 filename.md -o output.html

Convert Markdown to Docs : pandoc -s filename.md -o output.docx

Convert Markdown to pdf  : pandoc -f markdown -t beamer filename.md -o output.pdf


