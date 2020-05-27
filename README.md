# Pandoc Letter Template (DIN 5008)

This template allows you to write simple letters in Markdown and convert them
into nice looking PDFs. The template is based on Koma Script and satisfies
the German DIN 5008 norm for letters.

## Update:
This fork supports `\tightlist`, `\section` and `\subsection` commands:
```markdown
# Section
## Subsection

Legacy List:

- Item

- Item

And this becomes a \tightlist:

- Item
- Item
```

### Usage

I did not follow the original advice, mine did compile just fine using 

`pandoc --template="letter.latex" example.md -o example.pdf`

### Example

See [example folder](https://github.com/lmzdev/pandoc-letter-din5008/tree/master/example) for results.

### Requirements

In order to use the template you must have installed the following components:

- [Pandoc](http://pandoc.org/installing.html)
- [LaTeX](https://latex-project.org/ftp.html)

### Configuration

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
