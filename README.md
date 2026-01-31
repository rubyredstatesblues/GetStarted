# GetStarted

# Markdown

* [How to Convert a Word Document to Markdown for Free using Pandoc](https://www.youtube.com/watch?v=HPSK7q13-40)
* [Download Software](https://github.com/jgm/pandoc)

That command is a compact little powerhouse, and each piece plays a
specific role. Breaking it down makes the whole thing feel much more
intuitive.

``` bash
pandoc -t gfm --extract-media . "fan guide.docx" -o main.md
```

**What the command does**

It converts a Word document (fan guide.docx) into a Markdown file
(main.md) using Pandoc, while also extracting any embedded images or
media into a separate folder.

**Breakdown of each part**

**pandoc**

- The universal document converter. It reads one format and outputs
  another.

**-t gfm**

- Sets the **target format**.

- gfm stands for **GitHub‑Flavored Markdown**.

- This ensures the output Markdown uses GitHub’s syntax rules (tables,
  fenced code blocks, task lists, etc.).

**--extract-media .**

- Tells Pandoc to extract all embedded media (images, audio, etc.) from
  the .docx file.

- The . means “put the extracted media in the current directory.”

- Pandoc will create a folder like media/ or fan_guide/media/ depending
  on the document.

**"fan guide.docx"**

- The **input file**.

- Quoted because it contains a space.

**-o main.md**

- The **output file**.

- Pandoc writes the converted Markdown to main.md.

**Summary**

You’re converting a Word document into GitHub‑Flavored Markdown and
pulling out all images/media into a folder in the current directory.

If you want, I can also explain how to customize the output, clean up
the media folder, or automate this for multiple files.


``` bash
pandoc -t gfm --extract-media . "fan guide.docx" -o main.md
```
