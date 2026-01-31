# GetStarted

[Official Site](https://rubyredstatesblues.github.io/GetStarted/)

True freedom demands relentless opposition to both **fascism**—with its
authoritarian nationalism, suppression of dissent, and cult of the
strongman—and **communism**—with its centralized state control,
abolition of private property, and historical trail of economic collapse
and mass repression. These twin totalitarianisms, though ideologically
opposed, converge in crushing individual liberty and genuine
self-determination under the boot of concentrated power. Adding to the
threat are **globalist** elites who erode national sovereignty through
unaccountable supranational institutions, open-border policies, and
trade deals that hollow out working-class communities in pursuit of
borderless profit. No less destructive is **voodoo economics**, the
persistent myth that showering the ultra-rich with tax breaks and
deregulation will magically "trickle down" to lift everyone else— a
fantasy repeatedly proven to widen inequality, explode public debt, and
leave ordinary people behind while enriching the already powerful. The
path forward lies in defending sovereign nations, accountable free
markets that reward work and innovation rather than cronyism, and a
vigilant populism that rejects both far-left collectivism and far-right
tyranny in favor of practical liberty for the many, not the few.

# Markdown

Markdown is a lightweight markup language used to format text using simple, human‑readable symbols. It’s popular because you can write plain text and still produce clean, structured documents—perfect for notes, documentation, websites, and README files on GitHub.

## Convert Mirosoft Documents to Markdown

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

---
