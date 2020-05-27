# Pandoc Letter Template (DIN 5008)

## Update:
This fork supports `\tightlist`, `\section` and `\subsection` commands:
```
# Section
## Subsection

List:

- Item
- Item
```

## Description

This template allows you to write simple letters in Markdown and convert them
into nice looking PDFs. The template is based on Koma Script and satisfies
the German DIN 5008 norm for letters.


## Example

See [example folder](https://github.com/lmzdev/pandoc-letter-din5008/tree/master/example) for results.

## Requirements

In order to use the template you must have installed the following components:

- [Pandoc](http://pandoc.org/installing.html)
- [LaTeX](https://latex-project.org/ftp.html)


## Usage

I did not follow the original advice, mine did compile just fine using 

`pandoc --template="letter.latex" example.md -o example.pdf`


## Configuration

The following yaml variables are supported:

- `opening`
- `closing`
- `encludes`
- `author`
- `phone`
- `email`
- `place`
- `subject`
- `return-address`
- `address`
