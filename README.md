# cs33-handout-converter
Convert 33 handouts (or others, for that matter) to various forms.

## Usage
You can use the convert handout script with various combinations of file conversions. Any unrecognized pairing will generate the following help menu:
```
usage: ./convert-handout --from [text|markdown] --to [markdown|html|foldable] file
Specify the input format and output format with --from and --to
These can also be -f and -t.

This utility only goes "one direction". That is, it goes from text towards more complicated
html. This journey involves text --> markdown --> html --> foldable html.

Thus these are valid:
--from markdown --to html
--from text --to foldable

While these are not:
--from html --to markdown
--from markdown --to text
```