# cs33-handout-converter
Convert cs33 handouts to web format.

## First, convert the Google Doc handout to markdown format
Follow [these steps](https://github.com/mangini/gdocs2md) to convert your google doc to markdown.

Then look over the main content and fix any errors. See [this page](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatshe) for a markdown cheatsheet. I recommend installing a markdown live preview plugin for your text editor of choice (e.g. I know it works on atom and vscode) to see what your output will look like 

## Then, Convert to html

First to get the script, you can run
```
curl https://raw.githubusercontent.com/gcantieni/cs33-handout-converter/master/convert-handout > convert-handout && chmod +x convert-handout
```

Then you can run the script on your markdown
```
./convert-handout file.md > project_name.html
```
This should make the page foldable. Then email to the head TAs so it can be included in the website.
