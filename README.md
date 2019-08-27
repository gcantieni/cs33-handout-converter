# cs33-handout-converter
Convert cs33 handouts from markdown to a form with buttons

## First, convert the Google Doc handout to markdown format
Follow [these steps](https://github.com/mangini/gdocs2md) to convert your google doc to markdown.

Then look over the main content and fix any errors. See [this page](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatshe) for a markdown cheatsheet. You can also install a live preview plugin for your text editor of choice to see a pdf of the output.

## Then, Convert to html
Run
```
pandoc --from markdown_strict --to html file.md
```
replacing `file.md` with your file name.

## Finally, make it foldable
Run
```
./convert-handout file.html
```
using the included script. This should make the page foldable. Then email to the head TAs so it can be included in the website.
